<template>
  <v-app>
    <Navbar />
    <v-main>
      <Title />
      <div class="spacer">
        <div class="spacer-line"></div>
      </div>

      <Projects />

      <div class="spacer">
        <div class="spacer-line"></div>
      </div>

      <About />
    </v-main>
  </v-app>
</template>

<script>
import Navbar from "./components/Navbar";
import Title from "./components/Title";
import Projects from "./components/Projects";
import About from "./components/About";

export default {
  name: "App",

  components: {
    Navbar,
    Title,
    Projects,
    About,
  },
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.spacer-line {
  border-radius: 50px;
  background-color: #858585;
  height: 3px;
  width: 95%;

  display: flex;
  align-self: center;
  margin-left: 2.5%;
}
.spacer {
  background-color: #161214;
}
</style>
