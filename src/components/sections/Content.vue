<template>
    <div class="content">
        <div class="container">
            <div class="title">
                <span>Current Series</span>
            </div>
            <div class="series">
                <Serie v-for="(serie, index) in series" :key="index" :serie="serie"/>
            </div>
            <div class="load">
                <span>Load More</span>
            </div>
        </div>
    </div>
</template>

<script>
import Serie from '../commons/Serie.vue'
import Series from '../../assets/objets/dc-comics.json'

export default {
    name: 'Content',
    components: {
        Serie
    },
    data() {
        return {
            series: Series
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

    .content {
        color: white;
        background-color: #1c1c1c;

        .title {

            span {
                display: inline-block;
                text-transform: uppercase;
                font-weight: bold;
                padding: 12px 20px;
                background-color: $mainColor;
                transform: translateY(-50%);
            }
        }

        .series {
            display: flex;
            flex-wrap: wrap;

            > * {
                width: calc(100% / 6 - 20px);
                margin: 20px 10px;
                cursor: pointer;
                transition: transform 0.6s;

                &:hover {
                transform: scale(1.1);
            }
            }
        }

        .load {
            text-align: center;
            padding: 30px 0;

            span {
                text-transform: uppercase;
                font-weight: bold;
                background-color: $mainColor;
                padding: 10px 40px;
                cursor: pointer;

                &:hover {
                    background-color: #2f65ad;
                }
            }
        }
    }
</style>