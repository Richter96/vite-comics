<script>
export default {
    name: 'ProductItems',
    props: {
        image: String,
        title: String
    }
}
</script>
<template>
    <div class="col">
        <div class="card">
            <div class="square">
                <img :src="image" class="card_img" alt="...">
            </div>
            <div class="card-body">
                <h5 class="card-title text-white">{{ title }}</h5>
                <p class="card-text"></p>
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped></style>