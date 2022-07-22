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
/* Generics */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

img {
  height: auto;
  max-width: 100%;
}

ul {
  list-style-type: none;
}

a{
  color: #000;
  text-decoration: none;
}

/* Utils */
.container{
  margin: 0 auto;
  max-width: 1400px;
}
</style>
