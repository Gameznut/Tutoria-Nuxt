<template>
  <div class="container">
    <vc-date-picker
      v-model="range"
      :value="null"
      color="blue"
      is-range
      is-dark
      :rows="3"
      :columns="4"
      :timezone="timezone"
      mode="dateTime"
    />
  </div>
</template>

<script>
export default {
  data() {
    return {
      range: {
        start: new Date(),
        end: new Date(2022, 1, 15),
      },
      timezone: "",
    };
  },
};
</script>

<style scoped>
.container {
  padding: 0 4rem;
  width: 50%;
  margin: 20px;
}
</style>