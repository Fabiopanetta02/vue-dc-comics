<template>
  <section >
    <div id="jumbotron">
      <div class="container relative">
        <div class="button-blue-absolute">
          <span>
          <a href="#">CURRENT SERIES</a> 
        </span>
        </div>
      </div>
    </div>
    <div id="products">
      <div class="container boxes">
        <ProductCard v-for="(product, i) in products" :key="i" :product-src="product.thumb" :product-title="product.series"/>
      </div>
      <div class="button-blue">
        <span>
          <a href="#">LOAD MORE</a> 
        </span>
      </div>
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
#jumbotron{
  background-image: url(../assets/img/jumbotron.jpg);
  height: 400px;
  background-size: cover;

  .relative{
    position: relative;

    .button-blue-absolute{
      position: absolute;
      top: 380px;
      left: -15px;

      span{
        background-color: $active_color;
        padding: 15px 30px;

        a{
          color: $white;
          font-weight: bold;
          font-size: 22px;
        }
      }
    }
  }
}

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