<template>
  <div>
    <BaseHeader />
    <BaseMain />
    <BaseFooter />
  </div>
</template>

<script>
import BaseHeader from './components/BaseHeader.vue';
import BaseMain from './components/BaseMain.vue';
import BaseFooter from './components/BaseFooter.vue'
export default {
  name: 'DComics',
  components : {
    BaseHeader,
    BaseMain,
    BaseFooter
  }
}
</script>

<style lang="scss">
@import './assets/sass/style.scss';
</style>
