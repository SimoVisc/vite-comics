<script>
export default {
  name: "AppCard",
  props: {
    img: String,
    title: String,
  },
};
</script>

<template>
  <div class="card">
    <img :src="img" :alt="title" />
    <h3>{{ title }}</h3>
  </div>
</template>

<style lang="scss" scoped>
    .card {
        width:15%;
        margin:5px;
        
        img{
            width:80%
        }
    }
</style>