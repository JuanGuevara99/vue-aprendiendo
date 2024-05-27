<template>

<HeaderComp />
<router-view />
<FooterCom />
</template>

<script>
// Importar archivos de componentes
import HeaderComp from "./components/HeaderComp.vue";
import FooterCom from "./components/FooterComp.vue"

export default {
  name: "App",
  components: {
    HeaderComp,
    FooterCom
  }
}
</script>

<style>
#app {
    color: #2c3e50;
}

</style>
