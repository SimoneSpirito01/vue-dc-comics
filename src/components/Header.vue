<template>
  <header>
      <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="logo">
            </div>
            <nav>
                <ul>
                    <li><a href="#">Characters</a></li>
                    <li><a class="active" href="#">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">Tv</a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">Collectibles</a></li>
                    <li><a href="#">Videos</a></li>
                    <li><a href="#">Fans</a></li>
                    <li><a href="#">News</a></li>
                    <li><a href="#">Shop</a></li>
                </ul>
            </nav>
      </div>
  </header>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';

.container {
    height: 120px;
    display: flex;
    justify-content: space-between;
    align-items: center;

    img {
        width: 70px;
    }

    ul {
        font-size: 14px;
        text-transform: uppercase;
        list-style: none;
        display: flex;

        a {
            display: block;
            height: 120px;
            line-height: 120px;
            color: #1c1c1c;
            font-weight: bold;
            text-decoration: none;
            margin: 0 10px;

            &.active, &:hover {
                color: $mainColor;
                border-bottom: 4px solid $mainColor;
            }
        }
    }
}

</style>