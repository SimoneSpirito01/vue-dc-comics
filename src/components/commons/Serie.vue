<template>
    <div class="serie">
        <div class="image">
            <img :src="serie.thumb" :alt="serie.series">
        </div>
        <div class="text">
            <span>{{serie.series}}</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Serie',
    props: {
        serie: Object
    }
}
</script>

<style lang="scss" scoped>
    img {
        width: 100%;
        aspect-ratio: 0.9;
        object-fit: cover;
        object-position: top;
    }

    .text {
        margin-top: 10px;

        span {
        font-size: 12px;
        text-transform: uppercase;
        }
    }
</style>