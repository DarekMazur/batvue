<template>
  <footer class="footer">
    <p>Postać <span class='bat'>Batmana</span> stworzył Bob Kane</p>
    <p>{{ currentYear }} &copy {{ author }}</p>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      author: 'Gacek',
      currentYear: new Date().getFullYear()
    }

  }
}
</script>

<style lang="scss">
.footer {
  padding: 1.5rem 0;
  position: relative;
  display: flex;
  align-items: center;
  flex-direction: column;
  background: url('/assets/footer.jpg') no-repeat center center/cover;

  &::before {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    content: '';
    background-color: #505c7c;
    opacity: 0.7;
  }

  p {
    margin: 0;
    padding: 0;
    z-index: 1;
  }
}
</style>
