
<script>
import BannerVue from './BannerVue.vue';

export default {
    name: 'SiteMain',
    components: {
        BannerVue,
    },
    data() {
        return {

        }
    },
}
</script>


<template>
    <main id="app_main">
        <div class="container-md align-items-center">
            <p>CONTENT GOES HERE</p>
        </div>
        <BannerVue></BannerVue>
    </main>
</template>


<style lang="scss" scoped></style>