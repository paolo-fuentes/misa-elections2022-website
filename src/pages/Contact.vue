<template>
  <div>
    <div class="page-header clear-filter" filter-color="orange">
      <parallax
        class="page-header-image"
        style="background-image:url('img/bg5.jpg')"
      >
      </parallax>
      <div class="container">
        <div class="misa-logo">
          <img src="img/misa-logo.png" alt="" />
        </div>
        <h3 class="title">Contact eServices</h3>
      </div>
    </div>
    <div class="section">
      <div class="container">
        <h5 class="description">
          An artist of considerable range, Ryan — the name taken by
          Melbourne-raised, Brooklyn-based Nick Murphy — writes, performs and
          records all of his own music, giving it a warm, intimate feel with a
          solid groove structure. An artist of considerable range.
        </h5>

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
</style>
