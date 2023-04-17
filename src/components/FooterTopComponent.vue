<template>
    <section>
        <div id="footer_top">
            <div class="container">
                <ul class="list-unstyled d-flex justify-content-between">

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
            buyComicsFooter: buyComics
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