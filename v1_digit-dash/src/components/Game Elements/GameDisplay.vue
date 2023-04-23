<template>
  <div id="gameDisplay">
    <div class="grid">
      <Grid />
    </div>
    <div class="input-interface">
      <InputInterface />
    </div>
  </div>
</template>

<script>
import Grid from "./Grid.vue";
import InputInterface from "./InputInterface.vue";
export default {
  components: { Grid, InputInterface },
};
</script>

<style scoped>
#gameDisplay {
  width: 500px;
  margin: 5px auto;
}
.grid {
  margin: 5px auto;
}
.input-interface {
  margin: 100px auto 40px;
}
</style>
