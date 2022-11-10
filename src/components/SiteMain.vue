<script>
export default {
    name: 'SiteMain',
    data() {
        return {
            cards: [
                {
                    image: 'buy-comics-digital-comics.png',
                    text: 'digital comics'
                },
                {
                    image: 'buy-comics-merchandise.png',
                    text: 'dc merchandise'
                },
                {
                    image: 'buy-comics-subscriptions.png',
                    text: 'subscription'
                },
                {
                    image: 'buy-comics-shop-locator.png',
                    text: 'comic shop location'
                },
                {
                    image: 'buy-dc-power-visa.svg',
                    text: 'dc power visa'
                }
            ]
        }
    },
    methods: {
        getImagePath: function (imgPath) {
            return new URL(imgPath, import.meta.url).href;
        }
    },
}
</script>

<template>
    <main id="site_main">
        <div class="my-container">
            <div class="row row-cols-5">
                <div class="col d-flex align-items-center" v-for="card in cards">
                    <img :src="'/img/' + card.image" alt="">
                    <p>{{ card.text }}</p>
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss">

</style>
