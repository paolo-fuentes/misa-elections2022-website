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
            <h2 class="title">This page is coming soon</h2>
            <!-- <h5 class="description">
              eServices is a cluster under MISA that provides IT solutions to clients within and outside the organization. In line with MISA's vision of social transformation through information management, it aims to improve organizational processes of clients by delivering quality IT Solutions through the effective use of information technology.
            </h5>
            <h5 class="description">
              eServices is also a community of people who share the same passion for IT in MISA. Everyone is given the opportunity to foster their skills by taking on systems development projects, leveraging their technical expertise and equipping them with the competitive edge in the real world. At the same time, everyone is also engaged in creating bonds and building relationships among one another through uplifting the value of camaraderie and companionship.
            </h5> -->
          </div>
        </div>
      </div>

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
export default {
  data() {
    return {
      portfolio: [
        {
          title: "ORSEM 2020 Website",
          image: "/img/profile.jpg",
          status: "offline",
          tech_logos: [
            {
              image: "/img/techs/vue.png"
            },
            {
              image: "/img/techs/django.png"
            }
            

          ]
        },
        {
          title: "ORSEM 2020 Websites",
          link: "/profile",
          image: "/img/profile.jpg"
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
