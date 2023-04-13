<template>
    <header>
        <div class="container pt-5">
            <div id="img_container">
                <img src="../assets/img/dc-logo.png" alt="dc-logo">
            </div>
            <div id="navbar_container">
                <ul>
                    <li v-for="(link, index) in navbar" :key="index">
                        <a href="link.url" :class="{ 'active': link.current }">{{ link.text }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<script>
import { links } from '../assets/data/data.js'
export default {
    name: 'HeaderComponent',
    data() {
        return {
            navbar: links
        }
    }
}
</script>

<style lang="scss" scoped></style>