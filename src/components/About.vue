<template>
  <div class="about_section">
    <div id="title">
      <h1>
        About
      </h1>
    </div>
    <div class="content">
      <p class="about_text">
        My name is Lachie. I'm a fullstack developer who loves to learn.
      </p>
      <div class="skills">
        <h2>Skills</h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
};
</script>

<style>
/*
Colors:
- #161214
- white
- #D81E5B
- #858585
*/

.about_section {
  background-color: #161214;
  height: 100vh;
  display: flex;
  padding: 5rem 6rem;
}

.content {
  display: flex;
  justify-content: space-between;
  margin: 5rem;
  align-self: center;
  width: 100%;
}

#title {
  color: #d81e5b;
  font-size: 5vh;
  font-weight: bolder;
  align-self: center;
}

.about_text {
  color: white;
  font-size: 30px;
  width: 35%;
}

.skills {
  color: #d81e5b;
  font-size: 50px;
  display: flex;
  width: 100%;

  justify-content: center;
}
</style>
