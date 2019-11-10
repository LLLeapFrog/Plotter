<template>
  <div>
    <svg :height="size.height" :width="size.width">
      <rect :x="x" :y="y" :width="width" :height="height" :fill="colour" />
    </svg>
  </div>
</template>

<script>
export default {
  name: "R",
  props: ["size", "x", "y", "width", "height"],
  data() {
    return {
      colour: "#" + Math.floor(Math.random() * 16777215).toString(16)
    };
  }
};
</script>

<style scoped>
</style>