<template>
  <div>
    <div title="Using Component Methods">
      <button class="mt-3" block @click="() => {
          addItem(product.id) 
          display()}">
        Order
      </button>
      <div v-show="sent" class="bg-green-400 p-3 mt-6 rounded-2xl">
        <h1>Sent to MY ITEMS</h1>
      </div>
    </div>
  </div>
</template>

<script>
import { mapMutations } from "vuex";
export default {
  props: ["product"],
  data() {
      return {
          sent: false
      }
  },
  methods: {
    ...mapMutations(["addItem"]),
    display() {
        this.sent = true
        setTimeout(()=>{this.sent = false}, 2000)
    },
  },
};
</script>


<style scoped>
button {
  width: 100%;
  border: none;
  padding: 0.5rem;
  color: white;
  font-weight: 700;
  padding: 1rem 4rem;
  border-radius: 100rem;
  background-color: rgb(231, 81, 43);
  color: white;
  font-weight: 700;
  transition: 0.5s;
}
.calendar-container {
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
}
p {
  color: grey;
}
.text-container {
  padding: 0.5rem;
}
</style>

