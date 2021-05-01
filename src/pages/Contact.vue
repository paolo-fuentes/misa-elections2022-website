<template>
  <div>
    <div class="page-header clear-filter" filter-color="primary">
      <parallax
        class="page-header-image"
        style="background-image:url('img/bg5.jpg')"
      >
      </parallax>
      <div class="container">
        <br>
        <br>
        <br>
        <br>
        <br>
        <div class="misa-logo">
          <img src="img/misa-logo.png" alt="" />
        </div>
        <h3 class="title">Contact eServices</h3>
      </div>
    </div>
    <div class="section">
      <div class="container">
        <div class="section section-nucleo-icons">
          <div class="container">
            <div class="row">
              <div class="col-lg-6 col-md-12">
                <h2 class="title">Get in touch with us!</h2>
                <a href="https://www.facebook.com/Ateneo.MISA" target="_blank" class="btn btn-primary btn-icon btn-round"
                  ><i class="fab fa-facebook-square"></i
                ></a>
                <a href="https://twitter.com/AteneoMISA/"  target="_blank" class="btn btn-primary btn-icon btn-round" 
                  ><i class="fab fa-twitter"></i
                ></a>
                <a href="https://www.instagram.com/ateneomisa/" target="_blank" class="btn btn-primary btn-icon btn-round"
                  ><i class="fab fa-instagram"></i
                ></a>
                <h5 class="description">
                  <b>MISA WEBSITE: </b><a href="https://misa.org.ph/" target="_blank">misa.org.ph</a>
                  <br>
                  <b>EMAIL: </b> eservices@misa.org.ph
                  <br>
                  <b>ADDRESS:</b> 304 Manuel V. Pangilian Center for Student Leadership
                  Ateneo de Manila University, Katipunan Avenue
                  Loyola Heights, Quezon City 1108
                </h5>
              </div>
              <div class="col-lg-6 col-md-12">
                <div class="icons-container">
                  <i class="now-ui-icons ui-1_send"></i>
                  <i class="now-ui-icons ui-2_like"></i>
                  <i class="now-ui-icons business_chart-bar-32"></i>
                  <i class="now-ui-icons users_single-02"></i>
                  <i class="now-ui-icons design-2_html5"></i>
                  <i class="now-ui-icons emoticons_satisfied"></i>
                  <i class="now-ui-icons design_vector"></i>
                  <i class="now-ui-icons objects_spaceship"></i>
                  <i class="now-ui-icons business_bulb-63"></i>
                  <i class="now-ui-icons ui-2_favourite-28"></i>
                  <i class="now-ui-icons design_palette"></i>
                  <i class="now-ui-icons design_app"></i>
                  <i class="now-ui-icons education_hat"></i>
                  <i class="now-ui-icons tech_laptop"></i>
                  <i class="now-ui-icons business_globe"></i>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="section section-contact-us text-center">
            <div class="container">
                <h2 class="title">Want to work with us?</h2>
                <p class="description">Your project is very important to us.</p>
                <div class="row">
                <div class="col-lg-6 text-center ml-auto mr-auto col-md-8">
                    <fg-input
                    class="input-lg"
                    placeholder="First Name..."
                    v-model="form.firstName"
                    addon-left-icon="now-ui-icons users_circle-08"
                    >
                    </fg-input>
                    <fg-input
                    class="input-lg"
                    placeholder="Email Here..."
                    v-model="form.email"
                    addon-left-icon="now-ui-icons ui-1_email-85"
                    >
                    </fg-input>
                    <div class="textarea-container">
                    <textarea
                        class="form-control"
                        name="name"
                        rows="4"
                        cols="80"
                        v-model="form.message"
                        placeholder="Type a message..."
                    ></textarea>
                    </div>
                    <div class="send-button">
                    <n-button type="primary" round block size="lg"
                        >Send Message</n-button
                    >
                    </div>
                </div>
                </div>
            </div>
            </div>
      </div>
    </div>
  </div>
</template>
<script>
import { Button, FormGroupInput } from '@/components';
export default {
    
  name: 'contact',
  bodyClass: 'profile-page',
  components: {
    [Button.name]: Button,
    [FormGroupInput.name]: FormGroupInput
  },
  data() {
    return {
      form: {
        firstName: '',
        email: '',
        message: ''
      }
    };
  }
};
</script>
<style lang="scss" scoped>
.misa-logo{
    height: auto;
    max-width: 256px;
    margin: auto;
}

.section-nucleo-icons{
  h2, h4, h5{
    text-align: left;
  }
  
}
</style>
