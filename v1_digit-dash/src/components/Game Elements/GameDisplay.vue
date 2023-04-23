<template>
  <div id="gameDisplay">
    <div class="grid">
      <Grid :selectedItem="selectedNumber" />
    </div>
    <div class="input-interface">
      <InputInterface @input="selectNumber" />
    </div>
  </div>
</template>

<script>
import Grid from "./Grid.vue";
import InputInterface from "./InputInterface.vue";
export default {
  components: { Grid, InputInterface },
  data() {
    return {
      selectedNumber: "",
    };
  },
  methods: {
    selectNumber(event) {
      console.log(event);
    },
  },
};
</script>

<style scoped>
#gameDisplay {
  width: 560px;
  margin: 5px auto;
}
.grid {
  margin: 5px auto;
}
.input-interface {
  margin: 50px auto 40px;
}
</style>
