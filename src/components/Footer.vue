<template>
    <footer>
        <div class="container">
            <div class="top">
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
            <div class="middle"></div>
            <div class="bottom"></div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang="scss" scoped>

footer {
    background-color: #2982f9;

    .top {
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


</style>