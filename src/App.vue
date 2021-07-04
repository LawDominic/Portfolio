<template>
  <div id="wrapper">
    <div class="banner"/>
    
    <nav class="navbar navbar-expand-lg navbar-dark bg-transparent ">
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item active px-4">
            <a class="nav-link" href="/">Home</a>
          </li>
          <li class="nav-item px-4">
            <a class="nav-link" href="#">About</a>
          </li>
          <li class="nav-item px-4">
            <a class="nav-link" href="#">Projects</a>
          </li>
          <li class="nav-item ps-4">
            <a class="nav-link" href="#">Contact</a>
          </li>
        </ul>
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

import About from './components/About.vue'
import Contact from './components/Contact.vue'
import HeaderAnimation from './components/HeaderAnimation.vue'
import Projects from './components/Projects.vue'
export default {
  name: 'App',
  components: {
    About,
    Contact,
    HeaderAnimation,
    Projects,
  }
}
</script>

<style>

footer {
  width: 100%;
  height: 50px;
  background-color: #651e3e;
  color: #EDEDED;
}

.footerText {
  padding: 15px;
  font-size: 14px;
}

#app {
  font-family: Montserrat,sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height:100vh;
}

#wrapper {padding: 0 25vh;}

/* Navigation */
.navbar {
  margin-top: 50px;
  text-align: right;
  background: none;
}

/* Header */
.banner {
  background-image: url('./assets/header.jpg');
  background-size: cover;
  background-position: cover;
  height: 1000px;
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
  color: #651e3e;
  display: inline-block;
}
/* Misc styling */


</style>
