<template>
    <section>
        <div id="jumbotron"></div>
    </section>
</template>

<script>
export default {
    name: 'JumbotronComponent'
}
</script>

<style lang="scss" scoped>
#jumbotron {
    background-image: url(../assets/img/jumbotron.jpg);
    height: 20rem;
    background-size: cover;
}
</style>