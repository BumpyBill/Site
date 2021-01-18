<template>
  <v-app>
    <Navbar />
    <v-main>
      <Title />
      <div class="spacer"></div>

      <Projects />
    </v-main>
  </v-app>
</template>

<script>
import Navbar from "./components/Navbar";
import Title from "./components/Title";
import Projects from "./components/Projects";

export default {
  name: "App",

  components: {
    Navbar,
    Title,
    Projects,
  },
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.spacer {
  border-radius: 5px;
  background-color: #858585;
  height: 3px;
  width: 95%;
  position: absolute;
  display: flex;
  align-self: center;
  margin-left: 2.5%;
}
</style>
