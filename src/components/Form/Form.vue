<template>
  <section class="form">
    <div class="form__wrapper">
      <Button
        v-for="button in buttons"
        :class="{ selected: selectedItem === button }"
        @click="select(button)"
        :key="button"
        :label="button"
        :version="version"
      />
      <div class="form__input">
        <input id="name" name="name" />
        <label for="name">Imię/Nick</label>
      </div>
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
      selectedItem: null,
    };
  },
  components: {
    Navigation,
    Button,
  },
  methods: {
    select(button) {
      this.selectedItem = button;
    },
  },
};
</script>

<style lang="scss" scoped>
input {
  width: 300px;
  font-size: 1rem;
}

label {
  left: calc(50% - 140px);
}
</style>
