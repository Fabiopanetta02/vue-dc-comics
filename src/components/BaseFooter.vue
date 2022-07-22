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
  </footer>
</template>

<script>
export default {
    name: 'BaseFooter'
}
</script>

<style>
footer{
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}

.footer-nav{
    display: flex;
}

.footer-col{
    flex-basis: calc(100% / 2);
    display: flex;
}

.footer-col-figure{
    justify-content: flex-end;
}

.footer-col-sm{
    padding: 50px 0;
    flex-basis: calc(100% / 3);
    color: #fff;
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
    color: #959587;
    font-size: 18px;
}
</style>