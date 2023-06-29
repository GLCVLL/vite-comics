<script>
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
}
</script>

<template>
    <main>
        <div class="container">
            <div class="content">
                <h2>-- Content goes here --</h2>
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
/*content*/
.content {
    height: 120px;
    display: flex;
    align-items: center;

    h2 {
        color: white;
    }
}

/*navbar*/
nav {
    height: 150px;
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