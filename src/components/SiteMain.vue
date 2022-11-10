<script>
export default {
    name: 'SiteMain',
    data() {
        return {
            cards: [
                {
                    image: 'buy-comics-digital-comics',
                    text: 'digital comics'
                },
                {
                    image: 'buy-comics-merchandise',
                    text: 'dc merchandise'
                },
                {
                    image: 'buy-comics-subscriptions',
                    text: 'subscription'
                },
                {
                    image: 'buy-comics-shop-locator',
                    text: 'comic shop location'
                }
            ]
        }
    }
}
</script>

<template>
    <main id="site_main">
        <div class="container">
            <div class="row row-cols-5">
                <div class="col" v-for="card in cards">
                    <img :src="'../assets/img/' + card.image + '.jpg'" alt="">
                    <h5>{{ card.text }}</h5>
                </div>
                <div class="col">
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    <h5>dc power visa</h5>
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss">
#site_main {
    background-color: lightblue;
}
</style>
