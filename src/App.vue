<template>
  <div id="wrapper">
    <div class="banner"/>
    <nav class="navbar navbar-expand-lg navbar-dark bg-transparent ">
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item active px-4">
            <a class="nav-link" href="#">HOME</a>
          </li>
          <li class="nav-item px-4">
            <a class="nav-link" href="#">About</a>
          </li>
          <li class="nav-item px-4">
            <a class="nav-link" href="#">Projects</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Contact</a>
          </li>
        </ul>
      </div>
    </nav>
    <header id="header-content">
      <p>My name is <span class="highlight">Dominic Law</span>.<br /></p>
      <p>I am currently in my <span class="highlight">final year</span> at Macquarie University<br /></p>
      <p>actively pursuing a career in the <span class="highlight">Software Development</span> <br /></p>
      <p>landscape and aiming to perfect my craft.</p>
    </header>
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
#wrapper {
  padding: 0 25vh;
}

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
  height: 100vh;
  width: 100%; 
  position: fixed; 
  display: flex;
  flex-direction: column;
  left: 0px; 
  top: 0px; 
  opacity: 90%;
  filter: brightness(20%);
  z-index: -1;
}


/* Header + Animations */
#header-content {
  width:100%;
  height: 100%;
  margin-top: 25%;
}

#header-content p {
  vertical-align: center;
  text-align: left;
  color: #EDEDED;
  font-family: 'Anonymous Pro', monospace;
  white-space: nowrap;
  overflow: hidden;
  border-right: .15em solid white;
}

#header-content p:nth-child(1) {
  width: 13em;
  -webkit-animation: type 3s steps(40, end);
  animation: type 3s steps(40, end);
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

#header-content p:nth-child(2) {
  width: 30.5em;
  opacity: 0;
  -webkit-animation: type 3s steps(40, end);
  animation: type 3s steps(40, end);
  -webkit-animation-delay:3s;
  animation-delay: 3s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

#header-content p:nth-child(3) {
  width: 30em;
  opacity: 0;
  -webkit-animation: type 3s steps(40, end);
  animation: type 3s steps(40, end);
  -webkit-animation-delay: 6s;
  animation-delay: 6s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

#header-content p:nth-child(4) {
  width: 22.5em;
  opacity: 0;
  -webkit-animation: type2 3s steps(40, end), blink .5s step-end infinite alternate;
  animation: type2 3s steps(40, end), blink .5s step-end infinite alternate;
  -webkit-animation-delay: 9s;
  animation-delay: 9s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

@keyframes type {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid white;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@-webkit-keyframes type {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid white;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@keyframes type2 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  100% {
    opacity: 1;
  }
}

@keyframes blink {
  50% {
    border-color: transparent;
  }
}
@-webkit-keyframes blink {
  50% {
    border-color: tranparent;
  }
}

/* Header highlighting */
.highlight {
  background-color: #651e3e;
  background-position: 0% 0%;
  background-size: 100% 100%;
  transition: background-position .5s, background-size .3s ease-in 3s;
}

#about {
  display: block;
  background-color: black;
}

/* Misc styling */


</style>
