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
                <h1 class="title">MISA Elections</h1>
                </div>
            </div>
        </div>
        <div class="section section-about-us">
            <div class="container">
                <Candidate>

                </Candidate>
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
        

    


    
    </div>
</template>
<script>
import Candidate from '../pages/components/Candidate.vue'
export default {
    components: {
        Candidate
    }
}
</script>
<style>
</style>