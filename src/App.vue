<script>
// importo i componenti 
import HeaderApp from './components/headerApp.vue'
import MainApp from './components/mainApp.vue'
import FooterApp from './components/footerApp.vue'

export default {
  components: {
    HeaderApp,
    MainApp,
    FooterApp,
  },

}

</script>


<template>
  <header>
    <HeaderApp />

  </header>

  <main>
    <MainApp />

  </main>

  <footer>
    <FooterApp />

  </footer>
</template>

<style scoped></style>
