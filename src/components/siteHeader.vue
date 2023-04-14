

<script>
export default {
    name: 'SiteHeader',
    data() {
        return {
            menu: [
                {
                    text: 'Characters',
                    heref: '#'
                }
            ]
        }
    },
}
</script>

<template>
    <header id="app_header">
        <div class="container-md d-flex align-items-center justify-content-between">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <nav class="nav justify-content-center">
                <a class="nav-link active" href="#" aria-current="page">CHARACTERS</a>
                <a class="nav-link " href="#">COMICS</a>
                <a class="nav-link " href="#">MOVIES</a>
                <a class="nav-link " href="#">TV</a>
                <a class="nav-link " href="#">GAMES</a>
                <a class="nav-link " href="#">COLLECTIBLES</a>
                <a class="nav-link " href="#">VIDEOS</a>
                <a class="nav-link " href="#">FANS</a>
                <a class="nav-link " href="#">NEWS</a>
                <a class="nav-link " href="#">SHOP</a>
            </nav>
        </div>
    </header>
</template>

<style lang="scss"></style>