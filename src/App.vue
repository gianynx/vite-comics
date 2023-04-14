<template>
  <HeaderComponent />
  <JumbotronComponent />
  <MainComponent />
  <FooterComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import JumbotronComponent from './components/JumbotronComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';
export default {
  name: 'App',
  components: {
    HeaderComponent,
    JumbotronComponent,
    MainComponent,
    FooterComponent
  }
}
</script>

<style lang="scss" scoped>
* {
  font-family: 'Chivo Mono', monospace;
}
</style>