<template>
  <div class="grid">
    <Row v-for="row in rows" :number="selectedItem"></Row>
  </div>
</template>

<script>
import Row from "./Row.vue";
export default {
  components: { Row },
  props: {
    selectedItem: String,
  },
  data() {
    return {
      rows: [[], [], [], [], [], [], []],
    };
  },
};
</script>

<style scoped>
.grid {
  width: 350px;
}
</style>
