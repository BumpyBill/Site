<template>
  <v-app>
    <Navbar />
    <v-main>
      <Title />
    </v-main>
  </v-app>
</template>

<script>
import Navbar from "./components/Navbar";
import Title from "./components/Title";

export default {
  name: "App",

  components: {
    Navbar,
    Title,
  },
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
</style>
