<template>
    <footer>
        <div class="top">
            
            <div class="container">
                <div class="item" v-for="(tag, index) in tags" :key="index">
                    <img :src="require(`../assets/img/${tag.url}`)" :alt="tag.title">
                    <div class="text">{{tag.title}}</div>
                </div>
            </div>
            
        </div>
        
        <div class="middle">

            <div class="container">
                <div class="links">
                    <div class="col">
                        <div class="col-top">
                            <h2>Dc Comics</h2>
                            <ul>
                                <li>Characters</li>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Games</li>
                                <li>Videos</li>
                                <li>News</li>
                            </ul>
                        </div>
                        <div class="col-bottom">
                            <h2>Shop</h2>
                            <ul>
                                <li>Shop DC</li>
                                <li>Shop DC Collectibles</li>
                            </ul>
                        </div>
                    </div>
                    <div class="col">
                        <h2>Dc</h2>
                        <ul>
                            <li>Terms Of Use</li>
                            <li>Privacy policy(New)</li>
                            <li>Ad choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Helps</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>
                    <div class="col">
                        <h2>Sites</h2>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
                </div>
                <div class="big-logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="big-logo">
                </div>
            </div>
                
        </div>

        <div class="bottom">
            <div class="container">
                <div class="sign-up">
                    Sign-up now!
                </div>
                <div class="social">
                    <span>follow us</span>
                    <img src="../assets/img/footer-facebook.png" alt="facebook-logo">
                    <img src="../assets/img/footer-twitter.png" alt="twitter-logo">
                    <img src="../assets/img/footer-youtube.png" alt="youtube-logo">
                    <img src="../assets/img/footer-pinterest.png" alt="pintarest-logo">
                    <img src="../assets/img/footer-periscope.png" alt="periscope-logo">
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    data(){
        return {
            tags: [
                {
                    url: 'buy-comics-digital-comics.png',
                    title: 'digital comics'
                },
                {
                    url: 'buy-comics-merchandise.png',
                    title: 'dc merchandise'
                },
                {
                    url: 'buy-comics-subscriptions.png',
                    title: 'subscription'
                },
                {
                    url: 'buy-comics-shop-locator.png',
                    title: 'comic shop locator'
                },
                {
                    url: 'buy-dc-power-visa.svg',
                    title: 'dc power visa'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';

.top {
    background-color: $mainColor;
    
    .container {
        display: flex;
        justify-content: space-around;

        .item {
            color: white;
            text-transform: uppercase;
            display: flex;
            align-items: center;
            padding: 40px 0;

            img {
                width: 50px;
                margin-right: 15px;
            }

            .text {
                font-size: 13px;
            }
        }
    }
}

.middle {
    color: white;
    background-image: url(../assets/img/footer-bg.jpg);

    .container {
        display: flex;
        justify-content: space-between;

        .links {
        display: flex;
        padding: 40px 0;

            .col {
                margin: 0 20px;

                h2 {
                    font-size: 20px;
                    text-transform: uppercase;
                    margin-bottom: 12px;
                }

                ul {
                    list-style: none;
                    font-size: 14px;

                    li {
                        margin: 5px 0;
                        color: #948f8f;
                    }
                }

                .col-top {
                    margin-bottom: 20px;
                }
            }
        }

        .big-logo {
            width: 45%;
            position: relative;
            overflow: hidden;

            img {
                width: 120%;
                max-width: 500px;
                position: absolute;
                right: 0;
                object-fit: cover;
                object-position: center;
                transform: translateY(-12%);
                overflow: hidden;
            }
        }

    }
}

.bottom {
    background-color: #303030;

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 20px 0;

        .sign-up {
            color: white;
            text-transform: uppercase;
            padding: 10px 15px;
            border: 2px solid $mainColor;
            cursor: pointer;

        }

        .social {
            display: flex;
            align-items: center;

            span {
                color: $mainColor;
                text-transform: uppercase;
                font-weight: bold;
                margin-right: 15px;
                cursor: pointer;

            }

            img {
                width: 35px;
                margin: 0 10px;
                cursor: pointer;
            }
        }
    }
}



</style>