<template>
  <div
    class="w-full flex justify-between px-4 py-2 border-b border-slate-500 sticky top-0"
  >
    <img class="h-12 w-20" src="/Digit-Dash-Logo.png" />
    <div class="self-center">
      <button
        v-for="button in buttons"
        :class="button.css"
        class="mx-2 py-1 px-2 rounded-md shadow-md border-slate-200"
      >
        {{ button.name }}
      </button>
    </div>
  </div>
</template>
<script setup lang="ts">
const buttons = [
  { name: "New Game", css: "bg-green-200 hover:bg-green-400" },
  { name: "How to Play", css: "bg-blue-200 hover:bg-blue-400" },
  { name: "Highscore", css: "bg-red-200 hover:bg-red-400" },
];
</script>
