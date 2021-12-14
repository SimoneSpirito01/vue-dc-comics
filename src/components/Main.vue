<template>
  <main>
        <Hero/>
        <Content/>
  </main>
</template>

<script>
import Hero from './sections/Hero.vue'
import Content from './sections/Content.vue'

export default {
    name: 'Main',
    components: {
        Hero,
        Content
    }
}
</script>

<style lang="scss" scoped>

main {

    
}

</style>