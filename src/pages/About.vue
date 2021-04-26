<template>
  <div>
    <div class="page-header page-header-small" filter-color="primary">
      <parallax
        class="page-header-image"
        style="background-image: url('img/bg6.jpg')"
      >
      </parallax>
      <div class="content-center brand">
        <div class="container">
          <img class="n-logo" src="img/now-logo.png" alt="" />
          <h1 class="title">About eServices</h1>
        </div>
      </div>
    </div>
    <div class="section section-about-us">
      <div class="container">
        <div class="row">
          <div class="col-md-8 ml-auto mr-auto text-center">
            <h2 class="title">Who we are?</h2>
            <h5 class="description">
              eServices is a cluster under MISA that provides IT solutions to clients within and outside the organization. In line with MISA's vision of social transformation through information management, it aims to improve organizational processes of clients by delivering quality IT Solutions through the effective use of information technology.
            </h5>
            <h5 class="description">
              eServices is also a community of people who share the same passion for IT in MISA. Everyone is given the opportunity to foster their skills by taking on systems development projects, leveraging their technical expertise and equipping them with the competitive edge in the real world. At the same time, everyone is also engaged in creating bonds and building relationships among one another through uplifting the value of camaraderie and companionship.
            </h5>
          </div>
        </div>
      </div>
    </div>
    <div class="section section-team text-center">
      <div class="container">
        
        <div class="team" v-for="ebyear in eb.slice(0,1)" :key="ebyear.year" :selected="index === 0">
          <div class="row">
                <h2 class="title">eServices Board of Executives and the Associates {{ebyear.year}}</h2>
                <br>
                <br>
                <br>
                <br>
                <br>
                <br>
                <div class="col-md-4" v-for="ebmember in ebyear.ebyear" :key="ebmember.name" >
                    <div class="team-player">
                        <img
                        :src= ebmember.image_link
                        alt="Thumbnail Image"
                        class="rounded-circle img-fluid img-raised"
                        />
                        <h4 class="title">{{ebmember.name}}</h4>
                        <p class="category text-primary">{{ebmember.position}}</p>
                    </div>
                </div>
          </div>
        </div>
        <br>
        <br>
        <br>
        <section class=".eservs-alumni-container">
            <h2 class="title">eServices Board of Executives and the Associates Alumni</h2>
            <br>
            <br>
            <br>
            <div class="team" v-for="ebyear in eb.slice(1)" :key="ebyear.year">
                <h3 class="title">A.Y. {{ebyear.year}}</h3>
                <br>
                <div class="row">
                    <div class="col-md-3" v-for="ebmember in ebyear.ebyear" :key="ebmember.name">
                        <div class="team-player">
                            <img
                            :src= ebmember.image_link
                            alt="Thumbnail Image"
                            class="rounded-circle img-fluid img-raised"
                            />
                            <h4 class="title">{{ebmember.name}}</h4>
                            <p class="category text-primary">{{ebmember.position}}</p>
                        </div>
                    </div>
                </div>
                <br>
                <br>
            </div>

        </section>
      </div>
    </div>

    


    
  </div>
</template>
<script>
import { Button, FormGroupInput } from '@/components';
export default {
  name: 'landing',
  bodyClass: 'landing-page',
  components: {
    [Button.name]: Button,
    [FormGroupInput.name]: FormGroupInput
  },
  data() {
    return {
        eb: [
            {
                year: "2020-2021",
                ebyear: [{
                    name: "John Arvin Enriquez",
                    position: "VP FOR ESERVICES",
                    image_link: "img/ryan.jpg"
                },
                {
                    name: "Lorenzo Migel Pinaroc",
                    position: "AVP FOR SYSTEMS DOCUMENTATIONS",
                    image_link: "img/ryan.jpg"
                },
                {
                    name: "Paolo Laxamana",
                    position: "AVP FOR IT PRODUCTS AND SERVICES",
                    image_link: "img/ryan.jpg"
                },
                {
                    name: "Renzo Timothy Tan",
                    position: "AVP FOR IT SKILLS TRAINING AND EVALUATION",
                    image_link: "img/ryan.jpg"
                },
                {
                    name: "Sophia Jarobel",
                    position: "OSG ASSOCIATE FOR ESERVICES",
                    image_link: "img/eva.jpg"
                }]
            },
            {
                year: "2019-2020",
                ebyear: [
                {
                    name: "Lorenzo Migel Pinaroc",
                    position: "VP FOR ESERVICES",
                    image_link: "img/ryan.jpg"
                },
                {
                    name: "Meg Tuason",
                    position: "AVP FOR SYSTEMS DOCUMENTATIONS",
                    image_link: "img/eva.jpg"
                    
                },
                {
                    name: "Paolo Fuentes",
                    position: "AVP FOR IT PRODUCTS AND SERVICES",
                    image_link: "img/ryan.jpg"
                },
                {
                    name: "Erin Yabut",
                    position: "AVP FOR IT SKILLS TRAINING AND EVALUATION",
                    image_link: "img/ryan.jpg"
                }]
            },
            {
                year: "2018-2019",
                ebyear: [
                {
                    name: "Francis Avancena",
                    position: "VP FOR ESERVICES",
                    image_link: "img/ryan.jpg"
                },
                {
                    name: "Meg Tuason",
                    position: "AVP FOR SYSTEMS DOCUMENTATIONS",
                    image_link: "img/eva.jpg"
                    
                },
                {
                    name: "Paolo Fuentes",
                    position: "AVP FOR IT PRODUCTS AND SERVICES",
                    image_link: "img/ryan.jpg"
                },
                {
                    name: "Erin Yabut",
                    position: "AVP FOR IT SKILLS TRAINING AND EVALUATION",
                    image_link: "img/ryan.jpg"
                }]
            },
            {
                year: "2017-2018",
                ebyear: [
                {
                    name: "Daniel Tiongson",
                    position: "VP FOR ESERVICES",
                    image_link: "img/ryan.jpg"
                },
                {
                    name: "Francis Avancena",
                    position: "AVP FOR SYSTEMS DOCUMENTATIONS",
                    image_link: "img/eva.jpg"
                    
                },
                {
                    name: "Royce Chan",
                    position: "AVP FOR IT PRODUCTS AND SERVICES",
                    image_link: "img/ryan.jpg"
                },
                {
                    name: "Carlo Ferrer",
                    position: "AVP FOR IT SKILLS TRAINING AND EVALUATION",
                    image_link: "img/ryan.jpg"
                }]
            }
        ]
    };
  }
};
</script>
<style lang="scss" scoped>
.description{
    color: #2c2c2c;
}
.section-team .team-player {
    margin-bottom: 40px !important;

    .title{
        margin-top: 16px;
    }
}
</style>
