<template>
  <div id="wrapper">
    <div class="banner" />

    <!-- Navigation bar -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-transparent ">
      <div class="container-xl">
        <a class="navbar-brand" href="/">Dominic Law</a>

        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarsExample07XL"
          aria-controls="navbarsExample07XL"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item active px-4">
              <a class="nav-link" href="/">Home</a>
            </li>
            <li class="nav-item px-4">
              <a class="nav-link" href="#about">About</a>
            </li>
            <li class="nav-item px-4">
              <a class="nav-link" href="#projects">Projects</a>
            </li>
            <li class="nav-item ps-4">
              <a class="nav-link" href="#contact">Contact</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <HeaderAnimation></HeaderAnimation>
  </div>
  <About></About>
  <Projects></Projects>
  <Contact></Contact>
  <footer>
    <p class="footerText">Made with ❤️ by Dominic Law</p>
  </footer>
</template>

<script>
import About from "./components/About.vue";
import Contact from "./components/Contact.vue";
import HeaderAnimation from "./components/HeaderAnimation.vue";
import Projects from "./components/Projects.vue";
export default {
  name: "App",
  components: {
    About,
    Contact,
    HeaderAnimation,
    Projects,
  },
};
</script>

<style>
#app {
  font-family: Montserrat, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#wrapper {
  padding: 0 25vh;
}

/* Navigation */
.navbar {
  margin-top: 5vh;
  text-align: right;
  background: none;
}

/* Header */
.banner {
  background-image: url("./assets/header.jpg");
  background-size: cover;
  background-position: cover;
  height: 100vh;
  width: 100%;
  position: fixed;
  display: block;
  left: 0px;
  top: 0px;
  opacity: 90%;
  filter: brightness(20%);
  z-index: -1;
}

.secHeading {
  padding: 4rem;
  font-weight: bolder;
  font-size: 2rem;
  color: #651e3e;
  display: inline-block;
}

/* Footer */
footer {
  width: 100%;
  height: 50px;
  background-color: #651e3e;
  color: #ededed;
}

.footerText {
  padding: 15px;
  font-size: 14px;
}

/* Media query */
@media (max-width: 575px) {
  #wrapper {
    padding: 0 5vh;
  }
  .secHeading {
    padding: 2rem;
    font-size: 20px;
  }
}
/* Small devices (landscape phones, 576px and up) */
@media (min-width: 576px) {
  #wrapper {
    padding: 0 10vh;
  }
  .secHeading {
    padding: 3rem;
  }
}

/* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) {
  #header-content {
    font-size: 10px;
  }
}

/* Large devices (desktops, 992px and up) */
@media (min-width: 992px) {
  #header-content {
    font-size: 10px;
  }
  .secHeading {
    padding: 4rem;
  }
}

/* X-Large devices (large desktops, 1200px and up) */
@media (min-width: 1200px) {
  #header-content {
    font-size: 10px;
  }
  .secHeading {
    padding: 4rem;
  }
}

/* XX-Large devices (larger desktops, 1400px and up) */
@media (min-width: 1400px) {
  #header-content {
    font-size: 10px;
  }
  .secHeading {
    padding: 4rem;
  }
}
</style>
