<template>
    <section id="contact">
        <h1 class="secHeading display-5">Get in touch!</h1>
        <p id="contact-content">
        If you would like to get in touch with me, I am available here!
        <br/><br/>
        <a href="mailto:contact@domlaw.me" target="_blank"><img src="../assets/email-logo.png" height="24" width="24"/></a>
        <a href="https://github.com/LawDominic" target="_blank"><img src="../assets/github-logo.png" height="24" width="24"/></a>
        <a href="https://www.linkedin.com/in/lawdominic/" target="_blank"><img src="../assets/linkedin-logo.png" height="24" width="24"/></a>
        </p>
    </section>
</template>

<script>

export default {
  name: 'Contact',
}
</script>

<style scoped>
#contact {
  background-color: #EDEDED;
  width: 100%;
  height: 300px;
  display: block;
}

#contact-content > a > img {
  margin-left: 1rem;
  text-align: center;
  fill: white;
}

/* Media query */
@media (max-width: 575px) {
    #contact-content {
        font-size: 10px;
    }
    #contact {
      height: 200px;
    }
}
/* Small devices (landscape phones, 576px and up) */
@media (min-width: 576px) {
    #contact-content {
        font-size: 10px;
    }
}

/* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) {
    #contact-content {
        font-size: 10px;
    }
}

/* Large devices (desktops, 992px and up) */
@media (min-width: 992px) {
    #contact-content {
        font-size: 14px;
    }
}

/* X-Large devices (large desktops, 1200px and up) */
@media (min-width: 1200px) {
    #contact-content {
        font-size: 16px;
    }
}

/* XX-Large devices (larger desktops, 1400px and up) */
@media (min-width: 1400px) {
    #contact-content {
        font-size: 20px;
    }
}
</style>