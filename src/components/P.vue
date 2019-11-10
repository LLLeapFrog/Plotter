<template>
  <div>
    <svg :height="size.height" :width="size.width">
      <polygon :points="points" :fill="colour" />
    </svg>
  </div>
</template>

<script>
export default {
  name: "P",
  props: ["size", "points"],
  data() {
    return {
      colour: "#" + Math.floor(Math.random() * 16777215).toString(16)
    };
  }
};
</script>

<style scoped>
</style>