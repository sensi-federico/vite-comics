<script>
export default {
    name: 'SiteHeader',
    data() {
        return {
            links: [
                {
                    name: 'characters',
                    link: '#'
                },
                {
                    name: 'comics',
                    link: '#'
                },
                {
                    name: 'movies',
                    link: '#'
                },
                {
                    name: 'tv',
                    link: '#'
                },
                {
                    name: 'games',
                    link: '#'
                },
                {
                    name: 'collectibles',
                    link: '#'
                },
                {
                    name: 'videos',
                    link: '#'
                },
                {
                    name: 'fans',
                    link: '#'
                },
                {
                    name: 'news',
                    link: '#'
                },
                {
                    name: 'shop',
                    link: '#'
                },
            ]
        }
    }
}
</script>

<template>
    <header id="site_header">
        <div class="container">
            <div class="nav">
                <div class="logo">
                    <img src="/img/dc-logo.png" alt="">
                </div>
                <div class="links">
                    <a href="#" v-for="link in links">{{ link.name }}</a>
                </div>
            </div>
        </div>
        <div class="jumbotron">
            <div class="container">
                <h1>--> Content goes here &lt--</h1>
            </div>
        </div>
    </header>
</template>

<style lang="scss">

</style>
