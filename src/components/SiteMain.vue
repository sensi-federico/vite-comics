<script>
import ComicsCard from './ComicsCard.vue'
import Comics from './data/Comics.js'

export default {
    name: 'SiteMain',
    components: {
        ComicsCard
    },
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
            ],
            comics: Comics
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
        <div class="shop">
            <div class="my-container">
                <div class="banner-top">
                    <h5>current series</h5>
                </div>
                <div class="row">
                    <ComicsCard v-for="comic in comics" :url="comic.thumb" :title="comic.series" />
                </div>
                <div class="load d-flex">
                    <button class="btn btn-load">Load more</button>
                </div>
            </div>
        </div>


        <div class="banner">
            <div class="my-container">
                <div class="row row-cols-5">
                    <div class="col d-flex align-items-center" v-for="card in cards">
                        <img :src="'/img/' + card.image" alt="">
                        <p>{{ card.text }}</p>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss">

</style>
