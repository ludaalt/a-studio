<template>
  <HeaderBlock />
  <ClientsBlock />
  <ServicesBlock />
</template>

<script>
import HeaderBlock from "./components/HeaderBlock";
import ClientsBlock from "./components/ClientsBlock";
import ServicesBlock from "./components/ServicesBlock";

export default {
  name: "App",
  components: { HeaderBlock, ClientsBlock, ServicesBlock },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
