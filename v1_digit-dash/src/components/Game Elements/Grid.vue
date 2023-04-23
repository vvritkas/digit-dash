<template>
  <div class="grid">
    <Row v-for="row in rows"></Row>
  </div>
</template>

<script>
import Row from "./Row.vue";
export default {
  components: { Row },
  data() {
    return {
      rows: [1, 2, 3, 4, 5, 6, 7],
    };
  },
};
</script>

<style scoped>
.grid {
  width: 350px;
}
</style>
