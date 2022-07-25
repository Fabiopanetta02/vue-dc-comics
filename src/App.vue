<template>
  <div>
    <BaseHeader />
    <main>
      <ProductSection />
    </main>
    <BaseFooter />
  </div>
</template>

<script>
import BaseHeader from './components/BaseHeader.vue';
import ProductSection from './components/ProductSection.vue';
import BaseFooter from './components/BaseFooter.vue'
export default {
  name: 'DComics',
  components : {
    BaseHeader,
    ProductSection,
    BaseFooter
  }
}
</script>

<style lang="scss">
@import './assets/sass/style.scss';
</style>
