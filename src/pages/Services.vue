<template>
  <div>
    <div class="page-header page-header-small" filter-color="primary">
      <parallax
        class="page-header-image"
        style="background-image: url('img/bg6.jpg')"
      >
      </parallax>
      <div class="content-center">
        <div class="container">
          <h1 class="title">IT Products and Services</h1>
        </div>
      </div>
    </div>
    <div class="section section-about-us">
      <div class="container">
        <div class="row">
          <div class="col-md-8 ml-auto mr-auto text-center">
            <h2 class="title">Want to work with us?</h2>
            

            <!-- <n-progress type="primary" :value="0" label="Consult"></n-progress>
            <p class="description"></p>

            <n-progress type="primary" :value="20" label="Gather Requirements"></n-progress>
            <p class="description"></p>

            <n-progress type="primary" :value="40" label="Design"></n-progress>
            <p class="description"></p>

            <n-progress type="primary" :value="60" label="Develop"></n-progress>
            <p class="description"></p>

            <n-progress type="primary" :value="80" label="Test"></n-progress>
            <p class="description"></p>

            <n-progress type="primary" :value="100" label="Deploy"></n-progress>
            <p class="description"></p> -->
          </div>
        </div>
      </div>
      <br>
      <br>
      <br>
      <br>
      <div class="container text-center">
        <h3>Check out the works from the people in eServices</h3>
        <div class="row">


          <div class="col-md-4 portfolio-item" v-for="site in portfolio" :key="site.title">
            <h4> {{ site.title }} </h4>
            <img :src= site.image alt="Image" class="img-raised" />
            
            <router-link
              :to= site.link
              class="btn btn-simple btn-primary btn-round"
              v-if="site.link"
              >Visit Site
            </router-link>
            <div
              class="btn btn-round btn-simple disabled-custom" 
              v-else
              >Site Offline
            </div>
            <div class="tech-stacks text-center">
              <div class="tech-stack col-md-2" v-for="tech in site.tech_logos" :key="tech.image">
                <img :src= tech.image alt="Image" class="tech-logo" />
              </div>
            </div>
          </div>
          
        </div>
      </div>


    </div>
  </div>
</template>

<script>
import { Progress } from '@/components';
export default {
  components: {
    [Progress.name]: Progress,
  },
  data() {
    return {
      portfolio: [
        {
          title: "ORSEM 2020 Website",
          image: "/img/profile.png",
          status: "offline",
          tech_logos: [
            
            

          ]
        },
        {
          title: "ORSEM 2020 Websites",
          link: "/profile",
          image: "/img/profile.png"
        }
      ]
    }
  }
};
</script>

<style lang="scss" scoped>


.portfolio-item{
  margin-top: 32px;
  margin-bottom: 64px;
}

.disabled-custom:hover{
  cursor: default !important;
  color: #999999 !important;
  border-color: #999999 !important;
}

.tech-stacks{
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  padding: 12px;

}
</style>
