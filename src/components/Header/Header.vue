<template>
  <header class="header"><h1 class="header__title">Jak dobrze znasz Zamaskowanego Krzyżowca?</h1></header>
</template>
<script>
import hero from '../../../public/assets/hero.jpg'
  export default {
    data() {
      return {
        hero
      }
    }
  }
</script>

<style lang="scss" scoped>
.header {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0;
  padding: 1rem;
  height: 40vh;
  background: url('/assets/hero.jpg') no-repeat center center/cover;

  &::before {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    content: '';
    background-color: #0e0e18;
    opacity: 0.7;
  }

  &__title {
    margin: 0;
    z-index: 1;
    color: #dbdbdc;
  }
}
</style>