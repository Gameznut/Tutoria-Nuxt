<template>
  <NuxtLink  :to="`/products/${card.id}`" class="card">
      <img :src="require(`@/assets/images/${card.image}`)" class="image" alt="">
      <h3 class="header">{{card.title}}</h3>
      <p class="snippet">{{ card.snippet }}</p>
  </NuxtLink>
</template>

<script>
export default {
    props: [
        'card'
    ]
}
</script>

<style scoped>
 .card {
        width: 31.5%;
        height: 35rem;
        border: none;
        overflow: hidden;
        padding: 0;
        cursor: pointer;
    }
    .image {
        height: 85%;
        width: 100%;
        overflow: hidden;
        border-radius: 0.5rem;
    }
    .header {
        font-size: 1.15rem;
        margin-top: 0.4rem;
    }
    .snippet {
        color: grey
    }
</style>