<template>
<div>
   <div class="container">
    <LargeCardDisplay
      v-for="cardInfo in largeCardInfo.slice(0, 1)"
      :key="cardInfo.id"
      :cardsSection="cardInfo"
    />
    <SmallCardDisplay
      v-for="cardInfo in smallCardInfo"
      :key="cardInfo.id"
      :cardsSection="cardInfo"
    />
  </div>   
</div>

</template>

<script>
import { largeCardSections, smallCardSections } from "@/assets/data.js";

export default {
  data() {
    return {
      smallCardInfo: smallCardSections,
      largeCardInfo: largeCardSections,
    };
  },
};
</script>

<style scoped>
.container {
  margin: 0 5.5%;
  width: 100%;
}
</style>