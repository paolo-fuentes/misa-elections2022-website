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

            <form @submit="handleSubmit">
              <label class="custom-field one">
                <input type="number" placeholder="Enter ID Number" v-model="id" onKeyPress="if(this.value.length==6) return false;" required/>
              </label>
              <button
                    type="submit"
                    class="btn btn-primary btn-round btn-lg btn-block"
                    >Login
              </button>
                  
            </form>

              <template slot="raw-content">
                <div class="card-footer text-center">
                  
                  <a
                    href="/"
                    class="btn btn-default btn-round btn-lg btn-block"
                    >Cancel</a
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
<style>

.custom-field {
  position: relative;
  font-size: 14px;
  border-top: 20px solid transparent;
  margin-bottom: 5px;
  --field-padding: 12px;
}

.custom-field input {
  border: none;
  -webkit-appearance: none;
  -ms-appearance: none;
  -moz-appearance: none;
  appearance: none;
  background: #f2f2f2;
  padding: var(--field-padding);
  border-radius: 3px;
  width: 250px;
  outline: none;
  font-size: 14px;
  color: white;
}

::placeholder {
  color: white;
}


/* ONE */
.custom-field.one input {
  background: none;
  border: 2px solid #ddd;
  transition: border-color 0.3s ease;
}

.custom-field.one input + .placeholder {
  left: 8px;
  padding: 0 5px;
}



</style>
