<template>
  <header id="header-content">
    <p>My name is <span class="highlight">Dominic Law</span>.<br /></p>
    <p>
      I am currently in my <span class="highlight">final year</span> at
      Macquarie University<br />
    </p>
    <p>
      actively pursuing a career in the
      <span class="highlight">Software Development</span> <br />
    </p>
    <p>landscape and aiming to perfect my craft.</p>
  </header>
</template>

<style scoped>
/* Header + Animations */
#header-content {
  width: 100%;
  height: 100%;
  margin-top: 25%;
  font-size: 18px;
  color: #ededed;
  display: inline-block;
}

#header-content p {
  vertical-align: center;
  text-align: left;
  color: #ededed;
  font-family: "Anonymous Pro", monospace;
  white-space: nowrap;
  overflow: hidden;
  border-right: 0.15em solid white;
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
  -webkit-animation-delay: 3s;
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
  -webkit-animation: type2 3s steps(40, end),
    blink 0.5s step-end infinite alternate;
  animation: type2 3s steps(40, end), blink 0.5s step-end infinite alternate;
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
    border-right: 0.15em solid white;
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
    border-right: 0.15em solid white;
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
  transition: background-position 0.5s, background-size 0.3s ease-in 3s;
}

/* Media query */
@media (max-width: 575px) {
  #header-content {
    font-size: 10px;
    padding: 0 0vh;
  }
}

/* Small devices (landscape phones, 576px and up) */
@media (min-width: 576px) {
  #header-content {
    font-size: 10px;
    padding: 0 7.5vh 0 0;
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
    font-size: 14px;
    padding: 0 20vh 0 0;
  }
}

/* X-Large devices (large desktops, 1200px and up) */
@media (min-width: 1200px) {
  #header-content {
    font-size: 16px;
    padding: 0 20vh 0 0;
  }
}

/* XX-Large devices (larger desktops, 1400px and up) */
@media (min-width: 1400px) {
  #header-content {
    font-size: 20px;
    padding: 0 0 0 20vh;
  }
}
</style>
