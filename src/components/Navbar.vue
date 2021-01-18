<template>
  <nav>
    <div v-on:click="toggleHamburger" class="hamburger">
      <div class="line"></div>
      <div class="line"></div>
      <div class="line"></div>
    </div>
    <ul class="nav-links">
      <li><a>Contact</a></li>
      <li><a>Projects</a></li>
      <li><a>About</a></li>
    </ul>
  </nav>
</template>

<script>
function toggleHamburger() {
  const navLinks = document.querySelector(".nav-links");
  const links = document.querySelectorAll(".nav-links li");
  const lines = document.querySelectorAll(".line");

  navLinks.classList.toggle("open");

  links.forEach((link) => {
    link.classList.toggle("fade");
  });

  lines.forEach((link) => {
    link.classList.toggle("open");
  });
}
export default {
  name: "Navbar",
  methods: { toggleHamburger },
};
</script>

<style scoped>
/*
Colors:
- #161214
- white
- #D81E5B
- #858585
*/

nav {
  height: 10vh;
  position: absolute;
  z-index: 2;

  width: 100%;
}

.line {
  width: 30px;
  height: 3px;
  background: #d81e5b;
  margin: 5px;
  border-radius: 5px;
  transition: background-color 0.5s ease;
}
.line.open {
  background: white;
}

.hamburger {
  position: absolute;
  cursor: pointer;
  right: 5%;
  top: 50%;
  transform: translate(-5%, -50%);
  z-index: 3;
}

.nav-links {
  display: flex;
  list-style: none;
  position: fixed;
  background: #d81e5b;
  height: 100vh;
  width: 100%;
  justify-content: space-around;
  align-items: center;
  flex-direction: column;
  clip-path: circle(0 at 75% -10%);
  -webkit-clip-path: circle(0 at 100% -10%);
  transition: all 1s ease-out;
  pointer-events: none;
}
.nav-links.open {
  clip-path: circle(2500px at 75% -10%);
  -webkit-clip-path: circle(2500px at 100% -10%);
  pointer-events: all;
}

.nav-links li {
  opacity: 0;
  transition: opacity 0.5s ease;
}

li.fade {
  opacity: 1;
}

.nav-links li a {
  font-size: 25px;
  color: white;
  text-decoration: none;
}
</style>
