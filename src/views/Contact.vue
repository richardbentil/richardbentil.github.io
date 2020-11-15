<template>
    <div>
        <div class="row py-5">
            <div class="col-12">
                <h3 class="text-center my-3">Contact</h3>
                <div class="card shadow border-0">
                    <div class="card-body">
                        <p v-if="error">{{ error }}</p>
                        <form @submit.prevent="sendEmail">
                            <div class="row">
                                <div class="col-md-6 col-sm-6 col-12 form-group">
                                    <label for="user_name">Name *</label>
                                    <input type="text" class="form-control" id="user_name" v-model="name" name="name" aria-describedby="helpId">
                                </div>
                                <div class="col-md-6 col-sm-6 col-12 form-group">
                                    <label for="user_email">Email *</label>
                                    <input type="email" class="form-control" id="user_email" v-model="email" name="email" aria-describedby="helpId">
                                </div>
                            </div>
                            <div class="form-group">
                                <label for="message">Message</label>
                                <textarea id="message" cols="50" rows="3" v-model="message" name="message" class="form-control">
                                </textarea>
                            </div>
                            <button type="submit" class="btn btn-primary my-3 float-right">Submit</button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import emailjs from 'emailjs-com';
export default {
  name: 'Contact',
  data() {
    return {
      name: '',
      email: '',
      message: '',
      error: ''
    }
  },
  methods: {
    sendEmail(e) {
    this.name == '' || this.email == '' || this.message == ''
    ? this.error = 'Fill in form fields'
      : emailjs.sendForm('service_7nx97d8', 'template_mrnf0ir', e.target,
        'user_CVViIy7AKHj4DJsfyveXI', {
          name: this.name,
          email: this.email,
          message: this.message
        })
        .then(() => {
            this.error = 'Email sent';        
            // Reset form field
            this.name = ''
            this.email = ''
            this.message = ''
        }, (error) => {
            this.error = 'Email not sent' + error;
        });
    }
  }
}

</script>
