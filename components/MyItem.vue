<template>
  <div class="item-container">
    <img :src="require(`@/assets/images/${item.image}`)" alt="" />
    <div class="text-container">
      <h4>{{ item.title }}</h4>
      <p class="">{{ item.description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: ["item"],
};
</script>

<style scoped>
.item-container {
  display: flex;
  margin: 1rem 0;
}
.text-container {
  padding: 0 1rem;
  width: 100%;
}
img {
  width: 30%;
  border-radius: 0.5rem;
  height: 11rem;
}
p {
  font-size: 0.8rem;
  color: grey;
}
</style>