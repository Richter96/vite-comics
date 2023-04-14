
<script>
import BannerVue from './BannerVue.vue';
import Cards from '../assets/data/dc-comics'


export default {
    name: 'SiteMain',
    components: {
        BannerVue,
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
                <div class="col" v-for="card in cards">
                    <div class="card" style="width:10rem;">
                        <img :src="card.thumb" class="card-img-top" alt="...">
                        <div class="card-body">
                            <h5 class="card-title">Card title</h5>
                            <p class="card-text"></p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <BannerVue></BannerVue>
    </main>
</template>


<style lang="scss" scoped>
#app_main {
    background-color: #1c1c1c;

    p {
        color: #ffffff;
    }

}
</style>