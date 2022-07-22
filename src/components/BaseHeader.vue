<template>
    <header>
        <div class="top-header"></div>
        <div class="container"> 
            <nav>
                <figure>
                    <a href="#">
                        <img src="../assets/img/dc-logo.png" alt="">
                    </a>
                </figure>
                <ul>
                    <li><a href="#">CHARACTERS</a></li>
                    <li class="active"><a href="#" class="active">COMICS</a></li>
                    <li><a href="#">MOVIES</a></li>
                    <li><a href="#">TV</a></li>
                    <li><a href="#">GAMES</a></li>
                    <li><a href="#">COLLECTIBLES</a></li>
                    <li><a href="#">VIDEOS</a></li>
                    <li><a href="#">FANS</a></li>
                    <li><a href="#">NEWS</a></li>
                    <li><a href="#">SHOP</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'BaseHeader',
}
</script>

<style scoped>
.top-header{
    background-color: #1C1C1C;
    height: 3vh;
}

nav{
    padding: 20px 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

ul {
    display: flex;
    align-items: center;
    height: 107px;
}

ul li {
    font-weight: bold;
    height: 100%;
    display: flex;
    align-items: center;
    cursor: pointer;
}

ul li a{
    padding: 0px 10px;
}

ul li.active,
ul li:hover{
    border-bottom: 5px solid #0282F9;
}

ul li a.active,
ul li a:hover{
    color: #0282F9;
}
</style>