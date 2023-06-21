<template>
  <section>
    <div class="formWrapper">
      <Button
        v-for="button in buttons"
        :key="button"
        :label="button"
        :version="version"
      />
      <input />
    </div>
    <Navigation />
  </section>
</template>

<script>
import Button from "../Button/Button.vue";
import Navigation from "../Navigation/Navigation.vue";

export default {
  data() {
    return {
      buttons: ["Easy", "Normal", "Hard"],
      version: "select",
    };
  },
  components: {
    Navigation,
    Button,
  },
};
</script>
