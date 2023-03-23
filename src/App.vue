<script>
// prima importo il componente indicandogli il percorso e il nome
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";
import Button from "./components/Button.vue";
// funzionalità
export default {
  data() {
    return {
      message: "Ehilà",
      mostraPulsante: true,
    };
  },
  // aggiungiamo il componente, FUORI dai data()
  // in un oggetto apposito chiamato "components"
  components: {
    Footer,
    Button,
  },

  methods: {},
};
</script>

<template>
  <div>
    <!-- chiamo il componente nel mio template -->
    <div class="container">
      <Navbar></Navbar>
    </div>

    <h1>Ciao a tutti!</h1>
    {{ message }}

    <div v-if="mostraPulsante" v-for="number in 10">
      <Button></Button>
    </div>

    <!-- chiamo l'altro componente -->
    <Footer> </Footer>
  </div>
</template>

<style scoped>
/* stile */

.container {
  display: flex;
  flex-flow: row;
  color: white;
}

Footer {
  color: grey;
}
</style>
