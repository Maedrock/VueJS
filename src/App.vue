<template>
  <div id="app">
      <app-header></app-header>
      <app-amorph v-bind:infos="infos"></app-amorph>
      <app-footer></app-footer>
      
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Amorph from "./components/Amorph";
export default {
  components: {
    "app-header": Header,
    "app-footer": Footer,
    "app-amorph": Amorph
  },
  data() {
    return {
      infos: [
        { name: "Furkan", age: "20", role: "Admin", show: false },
        { name: "Yasin", age: "20", role: "Admin", show: false },
        { name: "Zahir", age: "20", role: "Moderator", show: false },
        { name: "Mustafa", age: "20", role: "User", show: false },
        { name: "Anılcan", age: "20", role: "User", show: false },
        { name: "Bahu", age: "22", role: "User", show: false }
      ]
    };
  }
};
</script>

<style>
* {
  padding: 0px;
  margin: 0px;
}
</style>
