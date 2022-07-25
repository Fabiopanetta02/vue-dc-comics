<template>
  <section>
    <div class="container">
        <div class="banner-icons">
            <div v-for="(item, i) in bannerItems" :key="i" class="media">
                <a href="#">
                    <img :src="item.src" :alt="item.text">
                    <p class="media-text">{{item.text.toUpperCase()}}</p>
                </a>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'BottomSection',
    data(){
        return {
            bannerItems: [
                {
                    src: require("../assets/img/buy-comics-digital-comics.png"),
                    text: "Digital comics",
                    url: "#"
                },
                {
                    src: require("../assets/img/buy-comics-merchandise.png"),
                    text: "Dc Merchandise",
                    url: "#"
                },
                {
                    src: require("../assets/img/buy-comics-subscriptions.png"),
                    text: "Subscription",
                    url: "#"
                },
                {
                    src: require("../assets/img/buy-comics-shop-locator.png"),
                    text: "Comic Shop Locator",
                    url: "#"
                },
                {
                    src: require("../assets/img/buy-dc-power-visa.svg"),
                    text: "Dc Power Visa",
                    url: "#"
                },

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/sass/vars";
    section{
        background-color: $active_color;

        .banner-icons{
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 50px;
            
            a{
                display: flex;
                align-items: center;

                img{
                    width: 55px;
                    height: 65px;
                    margin-right: 10px;
                }

                p{
                    color: $white;
                }
            }
        }
    }

</style>