<template>
    <div class="col-lg-2 col-md-4 col-sm-6 d-flex">
        <div class="card">
            <div class="card-body">
                <div class="card-image">
                    <a href="#"><img :src="image" :alt="title"></a>
                </div>
                <div class="card-title text-uppercase fw-bold small text-white pt-3">
                    {{ title }}
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardComponent',
    props: ['image', 'title']
}
</script>

<style lang="scss" scoped>
img {
    height: 170px;
    width: 170px;
}

.card {
    border: none;
    background-color: #1c1c1c;
}
</style>