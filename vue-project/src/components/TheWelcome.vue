<template>
  <div>
    <button v-for="number in 10" :key="number" @click="handleClick(number)">
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