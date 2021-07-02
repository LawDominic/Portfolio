<template>
  <div class="banner">
    <img class="stretch" src="./assets/header.jpg"/>
    <!-- <div class="overlay">
      <img class="stretch" src="./assets/header.jpg"/>
    </div> -->
  </div>
  <nav class="navbar navbar-expand-lg navbar-dark bg-transparent ">
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav ms-auto px-5">
        <li class="nav-item active px-4">
          <a class="nav-link" href="#">Home</a>
        </li>
        <li class="nav-item px-4">
          <a class="nav-link" href="#">About</a>
        </li>
        <li class="nav-item px-4">
          <a class="nav-link" href="#">Projects</a>
        </li>
        <li class="nav-item px-4">
          <a class="nav-link" href="#">Contact</a>
        </li>
      </ul>
    </div>
  </nav>
  <div class="container">
      <h1>Hello World</h1>
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {
    
  }
}
</script>

<style>
#app {
  font-family: Arial, Helvetica, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.navbar {
  margin-top: 50px;
  text-align: right;
  background: none;
}
.banner {
  width: 100%; 
  height: 100%; 
  position: fixed; 
  left: 0px; 
  top: 0px; 
  z-index: -1;
  opacity: 90%;
}
.overlay {
  background-color: black;
}
.banner img {
  filter: brightness(20%)
}
.stretch {
  width:100%;
  height:100%;
}
</style>
