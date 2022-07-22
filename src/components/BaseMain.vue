<template>
  <main>
    <div class="top-main">
        <div class="container">
            <h2>Content goes here</h2>
        </div>
    </div>
  </main>
</template>

<script>
export default {
    name: 'BaseMain'
}
</script>

<style lang="scss" scoped>
@import "../assets/sass/vars";
.top-main{
    background-color: $bg_dark;
    padding: 50px 0;
    color: $white;
}
</style>