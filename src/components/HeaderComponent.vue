<template>
    <header>
        <div class="container pt-3 pb-3 d-flex justify-content-between">
            <div id="img_container">
                <a href="#"><img src="../assets/img/dc-logo.png" alt="dc-logo"></a>
            </div>
            <div id="navbar_container">
                <ul class="d-flex list-unstyled pt-5">
                    <li v-for="(link, index) in navbar" :key="index">
                        <a href="link.url" :class="{ 'active': link.current }"
                            class="px-3 text-decoration-none text-uppercase text-dark fw-bold">{{ link.text }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<script>
import { links } from '../assets/data/data.js';
export default {
    name: 'HeaderComponent',
    data() {
        return {
            navbar: links
        }
    }
}
</script>

<style lang="scss" scoped>
header {
    border-bottom: 1px solid;
}

.active {
    background-color: red;
}
</style>