<script>
export default {
    data() {
        return {

        }
    },
}
</script>

<template>
    <footer>
        <div class="footer-top">
            <div class="nav-list container">
                <!-- prima list-->
                <div class="nav-list-left">
                    <ul>
                        <li>
                            <a href="#">
                                <h3>DC COMICS</h3>
                            </a>
                        </li>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Comics</a>
                        </li>
                        <li>
                            <a href="#">Movies</a>
                        </li>
                        <li>
                            <a href="#">TV</a>
                        </li>
                        <li>
                            <a href="#">Games</a>
                        </li>
                        <li>
                            <a href="#">Videos</a>
                        </li>
                        <li>
                            <a href="#">News</a>
                        </li>
                        <!-- seconda lista-->
                        <ul>
                            <li>
                                <a href="#">
                                    <h3>SHOP</h3>
                                </a>
                            </li>
                            <li>
                                <a href="#">Shop DC</a>
                            </li>
                            <li>
                                <a href="#">Shop DC Collectibles</a>
                            </li>
                        </ul>
                    </ul>
                </div>
                <div class="nav-list-center">
                    <ul>
                        <li>
                            <a href="#">
                                <h3>DC</h3>
                            </a>
                        </li>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Comics</a>
                        </li>
                        <li>
                            <a href="#">Movies</a>
                        </li>
                        <li>
                            <a href="#">TV</a>
                        </li>
                        <li>
                            <a href="#">Games</a>
                        </li>
                        <li>
                            <a href="#">Videos</a>
                        </li>
                        <li>
                            <a href="#">News</a>
                        </li>
                        <li>
                            <a href="#">TV</a>
                        </li>
                        <li>
                            <a href="#">Games</a>
                        </li>
                        <li>
                            <a href="#">Videos</a>
                        </li>
                        <li>
                            <a href="#">News</a>
                        </li>
                    </ul>
                </div>
                <div class="nav-list-right">
                    <ul>
                        <li>
                            <a href="#">
                                <h3>SITES</h3>
                            </a>
                        </li>
                        <li>
                            <a href="#">Comics</a>
                        </li>
                        <li>
                            <a href="#">Movies</a>
                        </li>
                        <li>
                            <a href="#">TV</a>
                        </li>
                        <li>
                            <a href="#">Games</a>
                        </li>
                        <li>
                            <a href="#">Videos</a>
                        </li>
                        <li>
                            <a href="#">News</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container social-info">
                <button>SIGN-UP NOW!</button>
                <ul>
                    <li>
                        <a href="#">
                            <h3>FOLLOW US</h3>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/footer-facebook.png" alt="fb">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/footer-twitter.png" alt="twitter">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/footer-youtube.png" alt="yt">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/footer-periscope.png" alt="periscope">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
/*navv list*/
.nav-list {
    display: flex;

    .nav-list-center {
        margin: 0 20px;
    }
}

ul {
    li {
        a {
            text-decoration: none;
            color: grey;
            transition: 0.3s ease;

            &:hover {
                color: white;
            }

            h3 {
                color: white;
                padding: 15px 0;
            }
        }
    }
}

/* footer-bottom */
.social-info {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;

    ul {
        display: flex;
        align-items: center;

        li {
            a {
                h3 {
                    color: #0c7cec;
                    margin: 0 10px;
                }

                img {
                    margin: 0 10px;
                }
            }
        }
    }
}

button {
    background-color: transparent;
    border: 2px solid #0c7cec;
    padding: 5px;
    font-weight: bold;
    transition: 0.3s ease;
    color: white;

    &:hover {
        background-color: #0c7cec;
    }
}
</style>