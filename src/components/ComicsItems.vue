<script>
export default {
    name: 'ComicsItems',
    props: {
        image: String,
        title: String
    }
}
</script>
<template>
    <div class="col">
        <div class="card border-0">
            <div class="square">
                <img :src="image" class="card_img img-fluid" alt="...">
            </div>
            <div class="card_body pt-3">
                <span class="card-title text-white text-uppercase">{{ title }}</span>
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped></style>