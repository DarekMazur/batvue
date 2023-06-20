<template>
  <div class="navigation">
    <Button v-for="button in buttons" :key="button" :label="button" />
  </div>
</template>
<script>
import Button from "../Button/Button.vue";
export default {
  data() {
    return {
      buttons: ["Reset", "Start"],
    };
  },
  components: {
    Button,
  },
};
</script>

<style lang="scss" scoped></style>
