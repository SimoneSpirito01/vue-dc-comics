<template>
  <main>
      <div class="container">
          <div class="text">
              <span>--> Content Goes Here...</span>
          </div>
      </div>
  </main>
</template>

<script>
export default {
    name: 'Main'
}
</script>

<style lang="scss" scoped>

main {
    background-color: #1c1c1c;

    .container {
        height: 120px;
        display: flex;
        align-items: center;

        .text {
            font-size: 25px;
            color: white;
            
        }
    }
}

</style>