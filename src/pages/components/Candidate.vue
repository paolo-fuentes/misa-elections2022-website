<template>
<div>
    <div class="candidate-card" >
        <img src="img/candidate-image.png">
        <div class="candidate-card-text">
          <h4>{{name}}</h4>
          <h5>{{position}}</h5>
          <n-button type="primary" @click="modals.classic = true">
              View Platform
          </n-button>
        </div>
        
    </div>
    

    <!-- Classic Modal -->
    <modal :show.sync="modals.classic" headerClasses="justify-content-center">
      <h4 slot="header" class="title title-up">Platform</h4>
      <h4>{{name}}</h4>
      <h5>{{position}}</h5>
      <img src="img/candidate-image.png">
      <br>
      <br>
      <p>
        {{platform}}
      </p>
      <template slot="footer">
        <n-button type="danger" @click.native="modals.classic = false"
          >Close</n-button
        >
      </template>
    </modal>
</div>
    
</template>
<script>
import { Button, Modal } from '@/components';
export default {
    components: {
    Modal,
    [Button.name]: Button
  },
  data() {
    return {
      modals: {
        classic: false
      }
    };
  },
  props: {
    name: String,
    position: String,
    image: String,
    platform: String
  }
}
</script>
<style lang="scss" scoped>
    .candidate-card{
      // border: 1px solid #DDDDDD;
      // transition: 0.2s;
      
      // &:hover{
      //   border: 1px solid #149da1;
      //   cursor: pointer;
      // }

      h4{
        margin: 12px 0px;
      }

      h5{
        margin: 0;
      }

      .candidate-card-text{
        // padding: 8px;
      }
    }

    
</style>