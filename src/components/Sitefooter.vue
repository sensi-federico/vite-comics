<script>
export default {
    name: 'SiteFooter',
    data() {
        return {
            brands: [
                {
                    image: 'footer-facebook.png'
                },
                {
                    image: 'footer-periscope.png'
                },
                {
                    image: 'footer-pinterest.png'
                },
                {
                    image: 'footer-twitter.png'
                },
                {
                    image: 'footer-youtube.png'
                },
            ]
        }
    }
}
</script>

<template>
    <footer id="site_footer">
        <div class="container d-flex align-items-center justify-content-between">
            <div class="button text-white">SIGN-UP NOW!</div>
            <div class="icons d-flex">
                <h4>Follow us</h4>
                <div class="brands ps-3" v-for="logo in brands">
                    <img :src="'/img/' + logo.image" alt="">
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss">

</style>