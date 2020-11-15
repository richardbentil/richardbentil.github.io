<template>
    <div>
        <footer>
            <div id="footer">
                <div class="container py-4">
                    <address>
                    <ul class="list-inline float-right pb-5">
                        <li class="list-inline-item mr-5">
                            <h6>Email</h6>
                            <router-link to="mailto:richardebo.bentil@gmail.com">richardebo.bentil@gmail.com</router-link>
                        </li>
                        <li class="list-inline-item">
                            <h6>Follow</h6>
                            <router-link to="https://www.linkedin.com/in/richard-bentil-636051115" target="_blank">
                            <i class="fa fa-linkedin fa-sm pr-2"></i>
                            </router-link><router-link to="https://web.facebook.com/bricks.murphy" target="_blank">
                            <i class="fa fa-facebook fa-sm pr-2"></i>
                            </router-link>
                        </li>
                    </ul>
                    </address>
                </div>
            </div>
        </footer>
    </div>
</template>
<script>
export default {
    name: "Footer"
}
</script>

