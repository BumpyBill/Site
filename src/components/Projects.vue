<template>
  <div class="projects_section">
    <div id="title">
      <h1>
        Projects
      </h1>
    </div>

    <div class="cards">
      <div class="card">
        <img class="card_img" src="@/assets/favicon.png" />

        <h3>
          <a href="https://bumpybill.me">
            PORTFOLIO
          </a>
        </h3>

        <div class="technologies">
          <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
              <img
                src="@/assets/vue.svg"
                class="icon"
                v-on="on"
                v-bind="attrs"
              />
            </template>
            <span>Vue</span>
          </v-tooltip>
          <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
              <img
                src="@/assets/vuetify.svg"
                class="icon"
                v-on="on"
                v-bind="attrs"
              />
            </template>
            <span>Vuetify</span>
          </v-tooltip>
          <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
              <img
                src="@/assets/netlify.svg"
                class="icon"
                v-on="on"
                v-bind="attrs"
              />
            </template>
            <span>Netlify</span>
          </v-tooltip>
          <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
              <img
                src="@/assets/github.svg"
                class="icon"
                v-on="on"
                v-bind="attrs"
              />
            </template>
            <span>Github</span>
          </v-tooltip>
        </div>
      </div>
      <div class="card">
        <img class="card_img" src="@/assets/plinco.png" />

        <h3>
          <a href="https://plinco.xyz">
            PLINCO
          </a>
        </h3>

        <div class="technologies">
          <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
              <img
                src="@/assets/nodejs.svg"
                class="icon"
                v-on="on"
                v-bind="attrs"
              />
            </template>
            <span>NodeJS</span>
          </v-tooltip>
          <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
              <img
                src="@/assets/heroku.svg"
                class="icon"
                v-on="on"
                v-bind="attrs"
              />
            </template>
            <span>Heroku</span>
          </v-tooltip>
          <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
              <img
                src="@/assets/github.svg"
                class="icon"
                v-on="on"
                v-bind="attrs"
              />
            </template>
            <span>Github</span>
          </v-tooltip>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Projects",
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

.projects_section {
  background-color: #161214;
  height: 100vh;
  display: flex;
  padding: 5rem 6rem;
}

#title {
  color: #d81e5b;
  font-size: 5vh;
  font-weight: bolder;
  align-self: center;
}

.cards {
  padding-left: 5vh;
  display: flex;
  align-self: center;
  justify-content: space-around;
  width: 100%;
}

.card {
  height: 300px;
  width: 250px;
  border-style: solid;
  border-radius: 5px;
  color: white;
  padding: 2rem;
  text-align: center;
}

.card h3 a {
  color: white;
  text-decoration: none;
}

.card_img {
  width: 100px;
  height: 100px;
  border-radius: 20px;
  margin-bottom: 1rem;
}
.technologies {
  display: flex;

  justify-content: space-between;
  align-content: space-around;
  padding: 2rem;
}
.icon {
  width: 30px;
  margin: 1px;
  height: 30px;
  filter: grayscale(100%);
}
</style>
