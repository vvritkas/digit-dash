<template>
  <div :class="customClass" @click="clickHandler">
    {{ number }}
  </div>
</template>

<script>
export default {
  props: {
    number: String,
    customClass: Array,
  },
  emits: ["click"],
  methods: {
    clickHandler(event) {
      this.$emit("click", event.target.outerText);
    },
  },
};
</script>

<style scoped>
.button {
  min-width: 40px;
  min-height: 40px;
  margin: 5px;
}
.digit {
  width: 40px;
  height: 40px;
  margin: 5px;
  cursor: default;
  display: inline-block;
  line-height: 40px;
  text-align: center;
  border: solid grey 1px;
  border-radius: 5px;
}

.right-position {
  background-color: green;
  color: white;
}

.right-digit {
  background-color: lightgreen;
}

.wrong {
  background-color: lightgray;
}
</style>
