<template>
  <section id="products">
    <div class="container boxes">
      <ProductCard v-for="(product, i) in products" :key="i" :product-src="product.thumb" :product-title="product.series"/>
    </div>
    <div class="button-blue">
      <span>
        <a href="#">LOAD MORE</a> 
      </span>
    </div>
  </section>
</template>

<script>
import ProductCard from './ProductCard.vue'
export default {
    name: 'ProductSection',
    components: {
      ProductCard
    },
    props: {
      products: Array
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/sass/vars";
#products{
    background-color: $bg_dark;
    padding: 50px 0;
    color: $white;

    .boxes{
      display: flex;
      flex-wrap: wrap;
    }

    .button-blue{
      text-align: center;

      span{
        text-align: center;
        background-color: $active_color;
        padding: 10px 30px;

        a{
          color: $white;
          font-weight: bold;
        }
      }
    }
    
}
</style>