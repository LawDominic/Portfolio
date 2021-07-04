<template>
    <section id="projects">
        <h1 class="secHeading display-5">Some things I've worked on</h1>
        <p id="projects-content">
        asdasasd
        </p>
    </section>
</template>

<script>

export default {
  name: 'About',
}
</script>

<style scoped>
    #projects {
    background-color: #EDEDED;
    width: 100%;
    height: 800px;
    display: block; 
    }

/* Media query */
@media (max-width: 575px) {
    #projects-content {
        font-size: 10px;
    }
}
/* Small devices (landscape phones, 576px and up) */
@media (min-width: 576px) {
    #projects-content {
        font-size: 10px;
    }
}

/* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) {
    #projects-content {
        font-size: 10px;
    }
}

/* Large devices (desktops, 992px and up) */
@media (min-width: 992px) {
    #projects-content {
        font-size: 14px;
    }
}

/* X-Large devices (large desktops, 1200px and up) */
@media (min-width: 1200px) {
    #projects-content {
        font-size: 16px;
    }
}

/* XX-Large devices (larger desktops, 1400px and up) */
@media (min-width: 1400px) {
    #projects-content {
        font-size: 20px;
    }
}
</style>