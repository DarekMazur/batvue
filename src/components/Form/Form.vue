<template>
  <div class="formWrapper">
    <Button v-for="button in buttons" :key="button" :label="button" />
    <input />
  </div>
</template>

<script>
import Button from "../Button/Button.vue";

export default {
  data() {
    return {
      buttons: ["Easy", "Normal", "Hard"],
    };
  },
  components: {
    Button,
  },
};
</script>
