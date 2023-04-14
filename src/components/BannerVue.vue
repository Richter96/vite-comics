<script>
export default {
    name: 'BannerVue',
    data() {
        return {
            banner: [
                {
                    titolo: 'Digital Comics',
                    src: 'buy-comics-digital-comics.png'
                },
                {
                    titolo: 'Digital Comics',
                    src: 'buy-comics-digital-comics.png'
                },
                {
                    titolo: 'Digital Comics',
                    src: 'buy-comics-digital-comics.png'
                },
                {
                    titolo: 'Digital Comics',
                    src: 'buy-comics-digital-comics.png'
                },
                {
                    titolo: 'Digital Comics',
                    src: 'buy-comics-digital-comics.png'
                },
                {
                    titolo: 'Digital Comics',
                    src: 'buy-comics-digital-comics.png'
                }
            ]
        }
    },
    mounted() {

    },
}
</script>


<template>
    <section class="banner">
        <div class=" container-md m-auto row">
            <div class="col">
                <a class=" text-decoration-none" href="">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                    <span class="text-white ps-3">DIGITAL COMICS</span>
                </a>
            </div>
            <div class="col">
                <a class=" text-decoration-none" href="">
                    <img src="../assets/img/buy-comics-merchandise.png" alt="">
                    <span class=" text-white ps-3">DC MERCHANDISE</span>
                </a>
            </div>
            <div class="col">
                <a class=" text-decoration-none" href="">
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                    <span class=" text-white ps-3">SUBSCRIPTIONS</span>
                </a>
            </div>
            <div class="col">
                <a class=" text-decoration-none" href="">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                    <span class=" text-white ps-3">COMIC SHOP LOCATOR</span>
                </a>
            </div>
            <div class="col">
                <a class=" text-decoration-none" href="">
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    <span class=" text-white ps-3">DC POWER VISA</span>
                </a>
            </div>

        </div>
    </section>
</template>


<style lang="scss" scoped></style>