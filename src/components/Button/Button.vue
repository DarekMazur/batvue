<template>
  <button :class="{ active: isActive }">
    {{ label }}
  </button>
</template>

<script>
const isActive = true;
export default {
  data() {
    return {
      isActive,
    };
  },
  props: ["label"],
};
</script>

<style lang="scss" scoped>
button {
  width: 10rem;
  height: 3rem;
  margin: 1rem 1.2rem;
  font-family: "Russo One", sans-serif;
}
</style>
