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
    <header id="header-content">
      <p>My name is <span class="highlight">Dominic Law</span>.<br /></p>
      <p>I am currently in my <span class="highlight">final year</span> at Macquarie University<br /></p>
      <p>actively pursuing a career in the <span class="highlight">Software Development</span> <br /></p>
      <p>landscape and aiming to perfect my craft.</p>
    </header>
  </div>
  <section id="about">
    <h1 class="secHeading display-5">Who am I?</h1>
    <p id="about-content">
      Hi! My name is Dominic Law. I'm currently in my final year at Macquarie<br/>
      University studying a Bachelor of Science with a major in Computing and <br/>
      a Bachelor of Commerce with a major in Finance. Currently looking for<br/>
      opportunities in the Software Development industry whether that is entry<br/>
      level, internships or graduate roles.
      <br/>
      <br/>
      Back in 2012, that was when my journey began, tinkering with websites<br/>
      and getting my hands dirty with HTML and CSS. Almost a decade later,<br/>
      I've expanded my skillset working with various languages for various<br/>
      specialities, including:<br/><br/>
      &#8226; Java<br/>
      &#8226; Python<br/>
      &#8226; JavaScript<br/>
      &#8226; HTML<br/>
      &#8226; CSS<br/>
      &#8226; SQL<br/><br/>
      
      These are also the frameworks I have tinkered with: <br/><br/>
      &#8226; React Native<br/>
      &#8226; Expo<br/>
      &#8226; Vue.js<br/>
      &#8226; Bootstrap<br/>
    </p>
  </section>
  <section id="projects">
    <h1 class="secHeading display-5">Some things I've worked on</h1>
    <p id="projects-content">
      asdasasd
    </p>
  </section>
  <section id="contact">
    <h1 class="secHeading display-5">Get in touch!</h1>
    <p id="contact-content">
      If you would like to get in touch with me, I am available here!
      <br/><br/>
      <a href="mailto:contact@domlaw.me" target="_blank"><img src="./assets/email-logo.png" height="24" width="24"/></a>
      <a href="https://github.com/LawDominic" target="_blank"><img src="./assets/github-logo.png" height="24" width="24"/></a>
      <a href="https://www.linkedin.com/in/lawdominic/" target="_blank"><img src="./assets/linkedin-logo.png" height="24" width="24"/></a>
    </p>
  </section>
  <footer>
    <p class="footerText">Made with ❤️ by Dominic Law</p>
  </footer>
</template>

<script>

export default {
  name: 'App',
  components: {
    
  }
}
</script>

<style>

#projects {
  background-color: #EDEDED;
  width: 100%;
  height: 800px;
  display: block;
}

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
  font-size: 18px;
  color: #EDEDED;
  display: inline-block;
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
  width: 12.5em;
  -webkit-animation: type 3s steps(40, end);
  animation: type 3s steps(40, end);
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

#header-content p:nth-child(2) {
  width: 30.3em;
  opacity: 0;
  -webkit-animation: type 3s steps(40, end);
  animation: type 3s steps(40, end);
  -webkit-animation-delay:3s;
  animation-delay: 3s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

#header-content p:nth-child(3) {
  width: 29.6em;
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
  margin-top: 20rem;
  background-color: #EDEDED;
  width: 100%;
  height: 800px;
  display: block;
}

.secHeading {
  padding: 4rem;
  font-weight: bolder;
  color: #651e3e;
  display: inline-block;
}

#contact {
  background-color: #EDEDED;
  width: 100%;
  height: 350px;
  display: block;
}

#contact-content > a > img {
  margin-left: 1rem;
  text-align: center;
  fill: white;
}

/* Misc styling */


</style>
