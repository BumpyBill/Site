<template>
  <v-app>
    <Navbar />
  </v-app>
</template>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
</style>

<script>
import Navbar from "./components/Navbar";

export default {
  name: "App",

  components: {
    Navbar,
  },

  data() {
    return {};
  },
};
</script>
