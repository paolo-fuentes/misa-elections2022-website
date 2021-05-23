<template>
  <div>
    <div class="page-header clear-filter" filter-color="primary">
      <parallax
        class="page-header-image"
        style="background-image:url('img/header.jpg')"
      >
      </parallax>
      <div class="container">
        <div class="content-center brand">
          <img class="n-logo" src="img/now-logo.png" alt="" />
          <h1 class="h1-seo">eServices</h1>
          <h3>Ateneo Management Information Systems Association</h3>
        </div>
      </div>
    </div>
    <div class="main">
      <div class="section section-images">
        <div class="container">
          <div class="row">
            <div class="col-md-12">
              <div class="hero-images-container">
                <img src="img/hero-image-1.png" alt="" />
              </div>
              <div class="hero-images-container-1">
                <img src="img/hero-image-2.png" alt="" />
              </div>
              <div class="hero-images-container-2">
                <img src="img/hero-image-3.png" alt="" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="section section-about-us">
      <div class="container">
        <div class="row">
          <div class="col-md-8 ml-auto mr-auto text-center">
            <h2 class="title">Who we are?</h2>
            <h5 class="description">
              We are from the Management Information Systems Association (MISA), the Ateneo Loyola Schools’ premier information management organization which serves as a home for MIS majors and like-minded IT enthusiasts. Founded in 1994, it is now on its 25th year of pursuing its main advocacy – social transformation through information management.
            </h5>
            <a
              href="/eservices"
              class="btn btn-primary btn-lg btn-simple btn-round"
              role="button"
            >
              Learn More
            </a>
          </div>
        </div>
        <div class="separator separator-primary"></div>
        <div class="section-story-overview">
          <div class="row">
            <div class="col-md-6">
              <div
                class="image-container image-left"
                style="background-image: url('img/login.jpg')"
              >
                <!-- First image on the left side -->
                <p class="blockquote blockquote-primary">
                  "The next step to business technology"
                  <br />
                  <br />
                  <!-- <small>-MISA</small> -->
                </p>
              </div>
              <!-- Second image on the left side of the article -->
              <div
                class="image-container"
                style="background-image: url('img/bg3.jpg')"
              ></div>
            </div>
            <div class="col-md-5">
              <!-- First image on the right side, above the article -->
              <div
                class="image-container image-right"
                style="background-image: url('img/bg1.jpg')"
              ></div>
              <h3>
                The next step to business technology.
              </h3>
              <p>
                We aim to be the country’s leading student organization of information management professionals leveraging our skills in information management for our pursuit of excellence and nation building. Guided by the core values of excellence, servant leadership and professionalism, we aim to inform, to form and to transform the society through proactive engagement in projects utilizing information technology as a tool towards effective information management. We provide a fun learning environment for our members to help them fully realize their potential as individuals and as catalysts of change through information management and information technology.
              </p>
              <p>
                MISA is among the 8 organizations of the Science and Technology Cluster of the Council of Organizations of the Ateneo. MISA is also a proud member of the Philippine Computing Organizations Alliance (PCOA).
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    
    <EservicesSection></EservicesSection>


  </div>
</template>
<script>
import { Parallax } from '@/components';
import  EservicesSection  from './components/EservicesSection.vue';

export default {
  name: 'index',
  bodyClass: 'index-page',
  components: {
    EservicesSection,
    Parallax,
  }
};
</script>
<style lang="scss" scoped>
.description{
    color: #2c2c2c;
}
</style>
