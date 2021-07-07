<template>
  <section id="projects">
    <h1 class="secHeading display-5">Some things I've worked on</h1>
    <p>WIP</p>
    <!-- <div class="container">
        <div class="row">
            <div class="col-sm-6">
                <h5 class="card-title">Special title treatment</h5>
                    <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eligendi, fugiat asperiores inventore beatae accusamus odit minima enim, commodi quia, doloribus eius! Ducimus nemo accusantium maiores velit corrupti tempora reiciendis molestiae repellat vero. Eveniet ipsam adipisci illo iusto quibusdam, sunt neque nulla unde ipsum dolores nobis enim quidem excepturi, illum quos!</p>
            </div>
            <div class="col-sm-3"><img src="https://picsum.photos/500/501"/></div>
        </div>
    </div> -->
  </section>
</template>

<script>
export default {
  name: "About",
};
</script>

<style scoped>

.row {
    background-color: white;
    border-radius: 10px;
    text-align: left;
    height: 300px;
}

.card-body {
    padding: 40px;
}

.card-title {
    font-weight: bold;
}

.card-text {
    margin-top: 20px;
    font-weight: normal;
}

.col-sm-12 {
    padding: 0;
    float: right;
    height: 300px;
}

#projects {
  background-color: #ededed;
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
