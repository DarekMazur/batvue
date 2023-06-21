<template>
  <button @click="$emit('click')" :class="version">
    {{ label }}
  </button>
</template>

<script>
let isActive = false;

export default {
  methods: {
    handleClick: function handleClick() {
      this.isActive = !this.isActive;
    },
  },
  data() {
    return {
      isActive,
    };
  },
  props: ["label", "version"],
};
</script>

<style lang="scss" scoped>
button {
  width: 10rem;
  height: 3rem;
  margin: 1rem 1.2rem;
  font-family: "Russo One", sans-serif;

  &.select {
    background-color: #021c25;
    color: #c4b61d;
  }

  &.selected {
    background-color: #c4b61d;
    color: #186c89;
  }
}
</style>
