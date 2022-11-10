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
        <div class="nav">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div class="links">
                <a href="#" v-for="link in links">{{ link.name }}</a>
            </div>
        </div>
        <div class="jumbotron">
            <h1>--> Content goes here &lt-- </h1>
        </div>
    </header>
</template>

<style lang="scss">
#site_header {

    .nav {
        display: flex;
        align-items: center;
        justify-content: space-around;
        padding: 1rem;

        .links {

            a {
                padding: .5rem;
                text-transform: uppercase;
                text-decoration: none;
                color: black;
            }
        }
    }

    .jumbotron {
        background-color: black;
        color: white;

        h1 {
            padding: 2rem;
            text-align: center;
        }
    }

}
</style>
