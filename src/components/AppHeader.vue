<script>
export default {
    data() {
        return {
            items: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ]
        }
    },
}
</script>

<template>
    <header>
        <div class="container" id="navbar-header">
            <figure class="logo">
                <img src="../assets/img/dc-logo.png" alt="logo">
            </figure>
            <ul>
                <li v-for="item in items" :key="item.text">
                    <a :href="item.url">{{ item.text }}</a>
                </li>
            </ul>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header {
    background-color: white;
    height: 120px;
}

header #navbar-header {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

ul {
    display: flex;

    li {
        a {
            text-decoration: none;
            color: black;
            padding: 5px;
            font-family: open sans condensed;

            &:hover {
                color: #0c7cec;
            }
        }
    }
}
</style>