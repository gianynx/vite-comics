<template>
    <section>
        <div id="footer_top">
            <div class="container d-flex justify-content-between">
                <ul class="list-unstyled">
                    <li v-for="(item, index) in buyComics" :key="index">
                        <img :src="item.icon" :alt="icon.text">
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<script>
import { buyComics } from '../assets/data/data.js';
export default {
    name: 'FooterTopComponent',
    data() {
        return {
            buyComics: buyComics
        }
    }
}
</script>

<style lang="scss" scoped>
#footer_top {
    height: 10rem;
    background-color: #0282f9;
}

img {
    color: white;
}
</style>