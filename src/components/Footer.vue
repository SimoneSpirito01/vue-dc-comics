<template>
    <footer>
        <div class="top">
            
            <div class="container">
                <div class="item">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="comics-digital">
                    <div class="text">Digital Comics</div>
                </div>
                <div class="item">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="comics-digital">
                    <div class="text">Digital Comics</div>
                </div>
                <div class="item">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="comics-digital">
                    <div class="text">Digital Comics</div>
                </div>
                <div class="item">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="comics-digital">
                    <div class="text">Digital Comics</div>
                </div>
                <div class="item">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="comics-digital">
                    <div class="text">Digital Comics</div>
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
                                <li>Comics</li>
                                <li>Comics</li>
                                <li>Comics</li>
                                <li>Comics</li>
                                <li>Comics</li>
                                <li>Comics</li>
                                <li>Comics</li>
                            </ul>
                        </div>
                        <div class="col-bottom">
                            <h2>Shop</h2>
                            <ul>
                                <li>Comics</li>
                                <li>Comics</li>
                            </ul>
                        </div>
                    </div>
                    <div class="col">
                        <h2>Dc</h2>
                        <ul>
                            <li>Terms Of Use</li>
                            <li>Terms Of Use</li>
                            <li>Terms Of Use</li>
                            <li>Terms Of Use</li>
                            <li>Terms Of Use</li>
                            <li>Terms Of Use</li>
                            <li>Terms Of Use</li>
                            <li>Terms Of Use</li>
                            <li>Terms Of Use</li>
                            <li>Terms Of Use</li>
                            <li>Terms Of Use</li>
                        </ul>
                    </div>
                    <div class="col">
                        <h2>Sites</h2>
                        <ul>
                            <li>MAD Magazine</li>
                            <li>MAD Magazine</li>
                            <li>MAD Magazine</li>
                            <li>MAD Magazine</li>
                            <li>MAD Magazine</li>
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
    name: 'Footer'
}
</script>

<style lang="scss" scoped>
$mainColor: #2982f9;

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
            width: 40%;
            position: relative;

            img {
                width: 120%;
                max-width: 500px;
                position: absolute;
                right: 0;
                object-fit: cover;
                object-position: center;
                transform: translateY(-12%);
            }
        }

    }
}

.bottom {
    background-color: #303030;
    position: relative;

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