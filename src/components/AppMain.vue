<script>
import ComicCard from './products/ComicCard.vue'
export default {
    data() {
        return {
            links: [
                {
                    text: 'DIGITAL COMICS',
                    url: '#',
                    image: 'buy-comics-digital-comics.png'
                },
                {
                    text: 'DC MERCHANDISE',
                    url: '#',
                    image: 'buy-comics-merchandise.png'
                },
                {
                    text: 'SUBSCRIPTION',
                    url: '#',
                    image: 'buy-comics-subscriptions.png'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    url: '#',
                    image: 'buy-comics-shop-locator.png'
                },
                {
                    text: 'DC POWER VISA',
                    url: '#',
                    image: 'buy-dc-power-visa.png'
                }
            ]
        }
    },
    components: { ComicCard },
    props: {
        products: Array
    }
}
</script>

<template>
    <main>
        <div class="jumbotron"></div>
        <div class="container">
            <div class="content">
                <h4>CURRENT SERIES</h4>
                <ComicCard v-for="product in products" :key="product.thumb" :product="product" />
                <div class="load-more">
                    <a href="#">LOAD MORE</a>
                </div>
            </div>
        </div>
        <nav>
            <div class="container">
                <ul>
                    <li v-for="link in links" :key="link.text">
                        <a :href="link.url">
                            <img :src="`../src/assets/img/${link.image}`" :alt="link.text">
                            <h3>{{ link.text }}</h3>
                        </a>
                    </li>
                </ul>
            </div>
        </nav>
    </main>
</template>

<style lang="scss" scoped>
.jumbotron {
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
}

/*content*/
.content {
    min-height: 500px;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    position: relative;

    h4 {
        background-color: #0c7cec;
        color: white;
        padding: 5px 10px;
        position: absolute;
        top: -3%;
        left: 0;
    }
}

/*CARD*/
.card {
    flex-basis: calc(100% / 6);
}

.load-more {
    margin: 30px auto;

    a {
        padding: 10px 15px;
        background-color: #0c7cec;
        color: white;
        text-decoration: none;
    }
}

/*navbar*/
nav {
    height: 120px;
    background-color: #0c7cec;

    .container {
        height: 100%;
    }
}

ul {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-around;

    li {
        display: flex;

        a {
            display: flex;
            align-items: center;
            text-decoration: none;
            color: white;
            font-family: open sans condensed;

            img {
                height: 50px;
                width: 50px;
                margin: 0 10px;
            }
        }
    }
}
</style>