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
            ],
            DcComics: [
                {
                    text: 'Characters'
                },
                {
                    text: 'Comics'
                },
                {
                    text: 'Movies'
                },
                {
                    text: 'TV'
                },
                {
                    text: 'Games'
                },
                {
                    text: 'Videos'
                },
                {
                    text: 'News'
                }
            ],
            Shop: [
                {
                    text: 'Shop DC'
                },
                {
                    text: 'Shop DC Collectibles'
                }
            ],
            DC: [
                {
                    text: 'Terms Of Use'
                },
                {
                    text: 'Privacy policy (New)'
                },
                {
                    text: 'Ad Choices'
                },
                {
                    text: 'Advertising'
                },
                {
                    text: 'Jobs'
                },
                {
                    text: 'Subscriptions'
                },
                {
                    text: 'Talent Workshops'
                },
                {
                    text: 'CPSC Certificates'
                },
                {
                    text: 'Ratings'
                },
                {
                    text: 'Shop Help'
                },
                {
                    text: 'Contact Us'
                },
            ],
            Sites: [
                {
                    text: 'DC'
                },
                {
                    text: 'MAD Magazine'
                },
                {
                    text: 'DC Kids'
                },
                {
                    text: 'DC Universe'
                },
                {
                    text: 'DC Power Visa'
                }
            ]
        }
    }
}
</script>

<template>
    <footer id="site_footer">

        <div class="contact">
            <div class="my-container">
                <div class="row">
                    <div class="col">
                        <div class="row">
                            <div class="col">
                                <h3>dc comics</h3>
                                <a href="#" v-for="item in DcComics">{{ item.text }}</a>

                                <h3>shop</h3>
                                <a href="#" v-for="item in Shop">{{ item.text }}</a>
                            </div>
                            <div class="col">
                                <h3>DC</h3>
                                <a href="#" v-for="item in DC">{{ item.text }}</a>
                            </div>
                            <div class="col">
                                <h3>Sites</h3>
                                <a href="#" v-for="item in Sites">{{ item.text }}</a>
                            </div>
                        </div>
                    </div>
                    <img class="logo-bg" src="/img/dc-logo-bg.png" alt="">
                </div>
            </div>

        </div>

        <div class="call-to-action">
            <div class="my-container d-flex align-items-center justify-content-between">
                <div class="button text-white">SIGN-UP NOW!</div>
                <div class="icons d-flex">
                    <h4>Follow us</h4>
                    <div class="brands ps-3" v-for="logo in brands">
                        <img :src="'/img/' + logo.image" alt="">
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss">

</style>