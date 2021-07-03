<template>
  <div id="wrapper">
    <div class="banner selectDisable">
      <img class="stretch" draggable="false" src="./assets/header.jpg"/>
    </div>
    <nav class="navbar navbar-expand-lg navbar-dark bg-transparent ">
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto px-5">
          <li class="nav-item active px-4">
            <a class="nav-link" href="#">HOME</a>
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
      <div id="header">
        <p class="typewriterAnim-1 line-1">My name is Dominic Law.<br /></p>
        <!-- <p class="typewriterAnim-2 line-2">I am a 4th year student actively<br /></p> -->
        <!-- <p class="typewriterAnim line">pursuing a career in the<br /></p>
        <p class="typewriterAnim line">Software Development landscape</p> -->
      </div>
    </div>
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
  padding: 0 15vh;
}

/* Navigation */
.navbar {
  margin-top: 50px;
  text-align: right;
  background: none;
}

/* Header */
.banner {
  width: 100%; 
  height: 100%; 
  position: fixed; 
  left: 0px; 
  top: 0px; 
  z-index: -1;
  opacity: 90%;
}

.banner img {
  filter: brightness(20%)
}
.stretch {
  width:100%;
  height:100%;
}
#header {
  text-align: left;
  color: #EDEDED;
  font-family: 'Anonymous Pro', monospace;
  background-color: rgb(25,25,25);
}
.line-1 {
  position: relative;
  border-right: 2px solid rgba(255, 255, 255, 0.75);
  overflow: hidden; transform: translateY(-50%);
  width: 20em;
  margin: 0 auto;
  white-space: nowrap;
}

.line-2 {
  position: relative;
  border-right: 2px solid rgba(255, 255, 255, 0.75);
  overflow: hidden; transform: translateY(-50%);
  width: 20em;
  margin: 0 auto;
  white-space: nowrap;
}

.typewriterAnim-1 {
  animation: typewriter-1 4s steps(40) 1s 1 normal both,
  blinkTextCursor 750ms steps(40) infinite normal;
}
.typewriterAnim-2 {
  animation: typewriter-2 4s steps(40) 5s 1 normal both,
  blinkTextCursor 750ms steps(40) infinite normal;
}
.typewriterAnim-3 {
  animation: typewriter 4s steps(40) 9s 1 normal both,
  blinkTextCursor 750ms steps(40) infinite normal;
}
.typewriterAnim-4 {
  animation: typewriter 4s steps(40) 13s 1 normal both,
  blinkTextCursor 750ms steps(40) infinite normal;
}

@keyframes typewriter-1 {
  from {
    width: 0;
  }
  to {
    width: 13em;
  }
}

@keyframes typewriter-2 {
  from {
    width: 0;
  }
  to {
    width: 18em;
  }
}

@keyframes blinkTextCursor {
  from {
    border-rigght-color: rgba(255, 255, 255, 0.75);
  }
  to {
    border-right-color: transparent;
  }
}
/* Misc styling */


</style>
