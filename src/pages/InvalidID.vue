<template>
  <div class="page-header clear-filter" filter-color="orange">
    <div
      class="page-header-image"
      style="background-image: url('img/login.jpg')"
    ></div>
    <div class="content">
      <div class="container">
        <div class="col-md-5 ml-auto mr-auto">
          <card type="login" plain>

            <h3>MISA EB Elections</h3>
            <div slot="header" class="logo-container">
              <img v-lazy="'img/now-logo.png'" alt="" />
            </div>
            <card plain></card>
            <h5>Sorry MISAn, you are not eligible to vote in this year's EB Elections.</h5>
              <template slot="raw-content">
                <div class="card-footer text-center">
                  <a
                    href="/"
                    class="btn btn-default btn-round btn-lg btn-block"
                    >Go Back to Home</a
                  >
                </div>
              
              </template>
  
          </card>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { Card, Button, FormGroupInput } from '@/components';
// import MainFooter from '@/layout/MainFooter';
export default {
  name: 'login-page',
  bodyClass: 'login-page',
  components: {
    Card,
    [Button.name]: Button,
    [FormGroupInput.name]: FormGroupInput
  },
  data() {
    return {
      id:"",
      idNumbers: ["182055", "182056"]
    }
  },
  methods: {
    handleSubmit() {
      if(this.idNumbers.includes(this.id)){
        this.$router.push("/ballot");
      }
      else{
        this.$router.push("/invalidID");
      }
      
    }
  }
};
</script>
<style></style>
