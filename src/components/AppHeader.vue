<script>
    import AppLogo from './AppLogo.vue';

    export default {
        name: "AppHeader",
        components:{
            AppLogo
        }
    }
</script>
<template>
  <header class="container">
     <AppLogo/>
     <nav class="main-nav">
            <ul>
                <li><strong><a href="">CHARACTERS</a></strong></li>
                <li><strong><a class="active" href="">COMICS</a></strong></li>
                <li><strong><a href="">MOVIES</a></strong></li>
                <li><strong><a href="">TV</a></strong></li>
                <li><strong><a href="">GAMES</a></strong></li>
                <li><strong><a href="">COLLECTIBLES</a></strong></li>
                <li><strong><a href="">VIDEOS</a></strong></li>
                <li><strong><a href="">FANS</a></strong></li>
                <li><strong><a href="">NEWS</a></strong></li>
                <li><strong><a href="">SHOP</a></strong></li>
            </ul>
      </nav>
  </header>
</template>

<style lang="scss" scoped>
 header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    text-align: center;
    padding: 10px;

    .main-nav {
        ul {
            display: flex;
            list-style: none;
            a{
            display: inline-block;
            margin: 10px;
            padding: 40px 0;
            font-size: 80%;
            text-decoration: none;
            &.active{
                border-bottom: var(--primary-color) solid 4px ;
            }
           }
        }
    }
 }
</style>