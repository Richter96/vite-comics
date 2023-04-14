
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
        <div class="jambotron">
            <img src="../assets/img/jumbotron.jpg" alt="">
        </div>
        <div class="container-md position-relative">
            <span class="badgeSeries text-uppercase">Current Series</span>
            <div class="row row-cols-6 mt-5">
                <ProductItems v-for="card in cards" :image="card.thumb" :title="card.series" />
            </div>
            <div class="d-flex justify-content-center">
                <button class="btn_load_more text-uppercase border-0 text-white fw-bold py-1 px-4 mb-3"> Load more</button>
            </div>
        </div>
        <BannerVue></BannerVue>
    </main>
</template>


<style lang="scss">
@use '../assets/scss/partials/variables' as *;

#app_main {
    background-color: #1c1c1c;

    .jambotron {
        width: 100%;
        max-height: 300px;
        overflow: hidden;

        img {
            object-fit: cover;
            max-width: 100%;
        }
    }

    .badgeSeries {
        background-color: #0c7cec;
        position: absolute;
        padding: 0.5rem 2rem;
        top: -62px;
        left: 0;
        color: white;
        font-weight: bold;
    }

    .col {
        margin: 1rem 0;
    }

    .btn_load_more {
        background-color: $primary;
    }

    .card {
        width: 100%;
        height: 100%;
        background-color: transparent;
        margin-bottom: 25px;

        .square {
            width: 100%;
            aspect-ratio: 1;
            overflow: hidden;
            box-shadow: 0 4px 8px 0 rgba(199, 199, 199, 0.463), 0 6px 20px 0 rgba(207, 207, 207, 0.19);

        }

        img {
            width: 100%;

        }
    }
}
</style>