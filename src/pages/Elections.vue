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
                <h1 class="title">MISA EB Elections</h1>
                </div>
            </div>
        </div>
        <div class="section section-about-us">
            <div class="container">
                <h3>Candidates</h3>
                <div class="candidates-container">
                    <div class="candidate-item" v-for="candidate in candidates" :key="candidate.name">
                        <Candidate
                            :name=candidate.name
                            :position=candidate.position
                            :image=candidate.image
                            :platform=candidate.platform
                        >
                        </Candidate>
                    </div>
                </div>

                <div class="vote-cta text-center">
                    <h3>Ready to vote?</h3>
                    <p><strong>Login with your ID number and if you're eligible to vote, you will be redirected to the form so you would be able to cast your vote.</strong></p>
                    <a
                    href="/elections-login"
                    class="btn btn-primary btn-lg btn-round btn-round"
                    role="button"
                    >
                        Vote
                    </a>
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
    },
    data() {
        return {
            candidates: [
                {
                    name: "Abigail Chua",
                    position: "President"
                },
                {
                    name: "Sophia Jarobel",
                    position: "Secretary General"
                },
                {
                    name: "Clarizza Castillo",
                    position: "Vice President for eServices"
                },
                {
                    name: "Luis Maningat",
                    position: "Vice President for Events"
                },
                {
                    name: "Jonwell Eufe Merit E",
                    position: "Vice President for HR"
                },
                {
                    name: "Kylie Marie Ong",
                    position: "Vice President for Marketing"
                },
            ]
        }
    }
}
</script>
<style lang="scss" scoped>
    .candidates-container{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(340px , 1fr));
        gap: 16px;
    }

    .vote-cta{
        margin: 64px auto ;
        max-width: 420px;
    }
</style>