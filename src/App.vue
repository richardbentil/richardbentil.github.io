<template>
  <div>
    <Navigation />
    <main>
    <div class="container">
    <div class="row">
    <div class="col-md-9 mx-auto" id="main-content">
      <router-view />
    </div>
    </div>
    </div>
    </main>
    <Footer />
  </div>
</template>
<script>
import Navigation from "@/components/Navigation.vue";
import Footer from "@/components/Footer.vue";
export default {
  components: {
    Navigation,
    Footer
  }
}
</script>

<style lang="scss">
@import "node_modules/bootstrap/scss/bootstrap";
</style>

