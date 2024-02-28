<template>
  <div class="button-grid">
    <button v-for="number in 9" :key="number" @click="handleClick(number)">
      {{ number }}
    </button>
  </div>
</template>

<script>
export default {
  methods: {
    handleClick(number) {
      console.log(`Button ${number} clicked`);
    },
  },
};
</script>

<style scoped>
.button-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 10px;
}
</style>