<template>
  <footer>
    <div class="container">
        <nav class="footer-nav">
            <div class="footer-col">
                <div class="footer-col-sm">
                    <h4>DC COMICS</h4>
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">Tv</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                    <h4>SHOP</h4>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>
                <div class="footer-col-sm">
                    <h4>DC</h4>
                    <ul>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshop</a></li>
                        <li><a href="#">CPSC Cerificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </div>
                <div class="footer-col-sm">
                    <h4>SITES</h4>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>
            </div>
            <div class="footer-col footer-col-figure">
                <figure>
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </figure>
            </div> 
        </nav>
    </div>
    <div class="bg-dark">
        <div class="container">
            <nav class="footer-nav-bottom">
                <div class="button-blue">
                    <a href="#">
                        <h3>SING-UP NOW!</h3>
                    </a>
                </div>
                <div class="social">
                    <div>
                        <h3>FOLLOW US</h3>
                    </div>
                    <figure>
                        <a href="#">
                            <img src="../assets/img/footer-facebook.png" alt="">
                        </a>
                        <a href="#">
                            <img src="../assets/img/footer-twitter.png" alt="">
                        </a>
                        <a href="#">
                            <img src="../assets/img/footer-youtube.png" alt="">
                        </a>
                        <a href="#">
                            <img src="../assets/img/footer-pinterest.png" alt="">
                        </a>
                        <a href="#">
                            <img src="../assets/img/footer-periscope.png" alt="">
                        </a>
                    </figure>
                </div>
            </nav>
        </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'BaseFooter'
}
</script>

<style lang="scss" scoped>
@import "../assets/sass/vars";
footer{
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;

    .footer-nav {
        display: flex;

        .footer-col{
            flex-basis: calc(100% / 2);
            display: flex;
            
            .footer-col-sm{
                padding: 50px 0;
                flex-basis: calc(100% / 3);
                color: $white;
            }

            .footer-col-sm h4{
                padding-bottom: 20px;
                font-size: 24px;
            }

            .footer-col-sm ul{
                padding-bottom: 20px;
            }

            .footer-col-sm ul li{
                margin-bottom: 5px;
            }

            .footer-col-sm ul li a {
                color: $light_grey;
                font-size: 18px;
            }
        
            &.footer-col-figure{
                justify-content: flex-end;
            }
        }
    }

    .bg-dark {
        background-color: $bg_dark;

        .footer-nav-bottom{
            display: flex;
            justify-content: space-between;
            align-items: center;

            .button-blue{
                border: 2px solid $active_color;
                margin: 50px 0;

                a h3 {
                    padding: 15px;
                    color: $white;
                }
            }

            .social{
                display: flex;
                align-items: center;

                h3{
                    color: $active_color;
                    margin-right: 10px;
                }  

                figure a img{
                    margin: 0 10px;
                }
            }
        }
    }
}
</style>