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

                </div>
            </div>
                
        </div>

        <div class="bottom">
            <div class="container">

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

.top {
    background-color: #2982f9;
    
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
        align-items: center;
        height: 350px;

        .links {
        display: flex;

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
                    }
                }

                .col-top {
                    margin-bottom: 20px;
                }
            }
        }

        .big-logo {
            width: 40%;
            height: 100%;
            background-image: url(../assets/img/dc-logo-bg.png);
            background-position: center;
            background-size: cover;
            transform: scale(1.1);
        }

    }
}



</style>