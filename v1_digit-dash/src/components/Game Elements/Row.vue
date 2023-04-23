<template>
  <div class="row">
    <Box
      v-for="digit in amountOfDigits"
      :number="number"
      :customClass="['digit']"
    ></Box>
  </div>
</template>

<script>
import Box from "./Box.vue";

export default {
  components: { Box },
  props: { number: String },
  data() {
    return {
      amountOfDigits: [1, 2, 3, 4, 5, 6, 7],
    };
  },
};
</script>

<style scoped>
.row {
  margin-bottom: 5px;
}
</style>
