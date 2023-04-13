<template>
    <header>
        <div class="container pt-3 d-flex justify-content-between">
            <div id="img_container">
                <a href="#"><img src="../assets/img/dc-logo.png" alt="dc-logo"></a>
            </div>
            <div id="navbar_container">
                <ul class="d-flex list-unstyled pt-5">
                    <li v-for="(link, index) in navbar" :key="index">
                        <a href="link.url" class="px-3 text-decoration-none text-uppercase fw-bold small text-dark">{{
                            link.text }}
                        </a>
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
    height: 9.6rem;
    border-bottom: 1px solid;
}

li {
    padding-bottom: 4rem;

    &:hover {
        border-bottom: 5px solid #0c7cec;
        cursor: pointer;
        padding: 1px;
    }
}
</style>