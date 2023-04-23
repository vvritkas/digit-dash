<template>
  <div class="input-interface">
    <Box v-for="number in numbers" :number="number"></Box>
  </div>
</template>

<script>
import Box from "./Box.vue";

export default {
  components: { Box },
  data() {
    return {
      numbers: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
    };
  },
};
</script>

<style scoped>
.row {
  margin-bottom: 15px;
}
</style>
