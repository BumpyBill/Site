<template>
  <div class="title_section">
    <h1>BumpyBill</h1>
    <Socials />
    <h2>I can code.</h2>
  </div>
</template>

<script>
import Socials from "./Socials";
export default {
  name: "Title",
  components: {
    Socials,
  },
};
</script>

<style>
.title_section {
  padding: 5rem 6rem;
  background-color: #161214;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.title_section h1 {
  font-weight: bolder;
  color: #d81e5b;
  font-size: 5rem;
}
.title_section h2 {
  font-weight: bolder;
  color: white;
  font-size: 3rem;
}
</style>
