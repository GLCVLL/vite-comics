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
        <figure class="logo">
            <img src="../assets/img/dc-logo.png" alt="logo">
        </figure>
        <ul>
            <li v-for="item in items" :key="item.text">
                <a :href="item.url">{{ item.text }}</a>
            </li>
        </ul>
    </header>
</template>

<style lang="scss" scoped>
/* header */
header {
    background-color: white;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: 20px 0;
}

ul {
    list-style-type: none;
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