<template>
  <main>
    <h3>{{ title }}</h3>
    <div>
      <p>
        Batman, Człowiek-Nietoperz, Zamaskowany Krzyżowiec, Mroczny Rycerz,
        Strażnik Gotham, Gacek. Postać-legenda. Uznany za największego bohatera
        wszechczasów przez magazyn SFX. Człowiek, któy pomimo braku supermocy (o
        ile za supermoc nie uznać liczby zer na koncie) jest w stanie pokonać
        najpotężniejszych przedstawicieli Universum DC. Dziś nadszedł czas, by
        sprawdzić swoją wiedzę o Człowieku-Nietoperzu. Pytania są podzielone na
        trzy kategorie - łatwe, normalne i trudne. Jednak jeżeli swoje
        informacje o Mrocznym Rycerzu czerpiesz z filmów, to w Arkham mają już
        przygotowaną celę.
      </p>
      <p>
        Przed Tobą 10 pytań. Czas rozruszać szare komórki i odpowiedzieć na
        pytanie - Jak dobrze znasz Zamaskowanego Krzyżowca!
      </p>
    </div>
    <Form />
  </main>
</template>
<script>
import Form from "../../components/Form/Form.vue";
export default {
  data() {
    return {
      title: "Zmierz się z Batmanem!",
    };
  },
  components: {
    Form,
  },
};
</script>
