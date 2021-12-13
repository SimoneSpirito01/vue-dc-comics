<template>
  <header>
      <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="logo">
            </div>
            <nav>
                <ul>
                    <li><a href="#">Movie</a></li>
                    <li><a class="active" href="#">Movie</a></li>
                    <li><a href="#">Movie</a></li>
                    <li><a href="#">Movie</a></li>
                    <li><a href="#">Movie</a></li>
                    <li><a href="#">Movie</a></li>
                    <li><a href="#">Movie</a></li>
                    <li><a href="#">Movie</a></li>
                    <li><a href="#">Movie</a></li>
                    <li><a href="#">Movie</a></li>
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
@import url('../assets/style/partials/variables.scss');
$mainColor: #2982f9;

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