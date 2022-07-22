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
                    <li v-for="voiceMenu in voicesMenu" :key="voiceMenu.text" :class="{active : voiceMenu.current}">
                        <a :href="voiceMenu.url" :class="{active : voiceMenu.current}">{{voiceMenu.text.toUpperCase()}}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'BaseHeader',
    data() {
        return {
            voicesMenu: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ]
        }
    }
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