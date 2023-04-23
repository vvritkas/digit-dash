<template>
  <div class="button">
    {{ number }}
  </div>
</template>

<script>
export default {
  props: {
    number: Number,
  },
};
</script>

<style scoped>
.button {
  width: 40px;
  height: 40px;
  margin: 5px;
}
</style>
