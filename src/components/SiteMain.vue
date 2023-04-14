
<script>
import BannerVue from './BannerVue.vue';
import ProductItems from './productItems.vue'
import Cards from '../assets/data/dc-comics'


export default {
    name: 'SiteMain',
    components: {
        BannerVue,
        ProductItems,
    },
    data() {
        return {
            cards: Cards
        }
    },
    mounted() {
        console.log(this.cards);
    },
}
</script>


<template>
    <main id="app_main">
        <div class="container-md ">
            <div class="row row-cols-6">
                <ProductItems v-for="card in cards" :image="card.thumb" :title="card.series" />

            </div>
        </div>
        <BannerVue></BannerVue>
    </main>
</template>


<style lang="scss">
#app_main {
    background-color: #1c1c1c;

    .card {
        width: 100%;
        background-color: transparent;
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
        margin-bottom: 25px;

        .square {
            width: 100%;
            aspect-ratio: 1;
            overflow: hidden;
        }

        img {
            width: 100%;

        }
    }

    p {
        color: #ffffff;
    }

}
</style>