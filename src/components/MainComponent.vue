<template>
    <main>
        <section class="container pt-5">
            <div class="row">
                <CardComponent :image="card.thumb" :title="card.series" v-for="(card, index) in comics" :key="index" />
            </div>
        </section>
    </main>
</template>

<script>
import { comics } from '../assets/data/comics';
import CardComponent from './CardComponent.vue';
export default {
    name: 'MainComponent',
    components: {
        CardComponent
    },
    data() {
        return {
            comics: [...comics]
        }
    }
}
</script>

<style lang="scss" scoped>
main {
    background-color: #1c1c1c;
}
</style>