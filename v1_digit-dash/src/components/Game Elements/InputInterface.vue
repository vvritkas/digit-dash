<template>
  <div class="input-interface">
    <div class="description title is-5">Bla bla bla</div>
    <Box
      v-for="element in inputelements"
      :number="element"
      :customClass="['button']"
      @click="inputHandler"
    ></Box>
  </div>
</template>

<script>
import Box from "./Box.vue";

export default {
  components: { Box },
  data() {
    return {
      inputelements: [
        "0",
        "1",
        "2",
        "3",
        "4",
        "5",
        "6",
        "7",
        "8",
        "9",
        "Delete",
        "Enter",
      ],
      inputArray: [],
    };
  },
  emits: ["input"],
  methods: {
    inputHandler(event) {
      if (
        event !== "Delete" &&
        event !== "Enter" &&
        this.inputArray.length < 7
      ) {
        this.inputArray.push(event);
        this.$emit("input", this.inputArray);
      } else if (
        event !== "Delete" &&
        event !== "Enter" &&
        this.inputArray.length === 7
      ) {
        this.inputArray[6] = event;
        this.$emit("input", this.inputArray);
      } else if (event === "Delete") {
        this.inputArray.pop();
        this.$emit("input", this.inputArray);
      } else if (event === "Enter") {
        let commitedDigits = { commit: true, digits: this.inputArray };
        this.$emit("input", commitedDigits);
      }
    },
  },
};
</script>

<style scoped>
.description {
  text-align: center;
}
</style>
