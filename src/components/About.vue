<template>
  <section id="about">
    <h1 class="secHeading">Who am I?</h1>
    <p id="about-content">
      Hi! My name is Dominic Law. I'm currently in my final year at Macquarie<br />
      University studying a Bachelor of Science with a major in Computing and
      <br />
      a Bachelor of Commerce with a major in Finance. Currently looking for<br />
      opportunities in the Software Development industry whether that is
      entry<br />
      level, internships or graduate roles.
      <br />
      <br />
      Back in 2012, that was when my journey began, tinkering with websites<br />
      and getting my hands dirty with HTML and CSS. Almost a decade later,<br />
      I've expanded my skillset working with various languages for various<br />
      specialities, including:<br /><br />
      &#8226; Java<br />
      &#8226; Python<br />
      &#8226; JavaScript<br />
      &#8226; HTML<br />
      &#8226; CSS<br />
      &#8226; SQL<br /><br />

      These are also the frameworks I have tinkered with: <br /><br />
      &#8226; React Native<br />
      &#8226; Expo<br />
      &#8226; Vue.js<br />
      &#8226; Bootstrap<br />
    </p>
  </section>
</template>

<script>
export default {
  name: "About",
};
</script>

<style scoped>
#about {
  margin-top: 20rem;
  background-color: #ededed;
  width: 100%;
  height: 800px;
  display: block;
}

/* Media query */
@media (max-width: 575px) {
  #about-content {
    font-size: 10px;
  }
  #about {
    height: 500px;
  }
}
/* Small devices (landscape phones, 576px and up) */
@media (min-width: 576px) {
  #about-content {
    font-size: 10px;
  }
}

/* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) {
  #about-content {
    font-size: 10px;
  }
}

/* Large devices (desktops, 992px and up) */
@media (min-width: 992px) {
  #about-content {
    font-size: 12px;
  }
}

/* X-Large devices (large desktops, 1200px and up) */
@media (min-width: 1200px) {
  #about-content {
    font-size: 14px;
  }
}

/* XX-Large devices (larger desktops, 1400px and up) */
@media (min-width: 1400px) {
  #about-content {
    font-size: 16px;
  }
}
</style>
