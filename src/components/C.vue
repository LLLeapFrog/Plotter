<template>
  <div>
    <svg :height="size.height" :width="size.width">
      <circle :cx="cx" :cy="cy" :r="r" :fill="colour" />
    </svg>
  </div>
</template>

<script>
export default {
  name: "C",
  props: ["size", "cx", "cy", "r"],
  data() {
    return {
      colour: "#" + Math.floor(Math.random() * 16777215).toString(16)
    };
  }
};
</script>

<style scoped>
</style>