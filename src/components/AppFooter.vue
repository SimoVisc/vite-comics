<script>
    export default {
    name: "AppFooter",
   }
</script>

<template>
  <div class="container-footer-top">
    <div class="container">
      <div>
        <h3>DC COMICS</h3>
        <ul>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
        </ul>
      </div>
   <img src="../assets/img/dc-logo.png" alt="logo">
  </div>
 </div>
</template>

<style lang="scss">
@use '../style/partials/mixin.scss' as *;
.container-footer-top{
  @include bg-img('../assets/img/footer-bg.jpg'); 
  padding:20px 0;
  .container{
    display: flex;
    justify-content: space-between;
  }
  li{
    color:gray;
    list-style: none;
  }
  img{
    width:30%;
    rotate: -40deg;
    opacity: 0.5
  }
}
</style>