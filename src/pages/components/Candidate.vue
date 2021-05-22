<template>
<div>
    <div class="candidate-card">
        <n-button type="primary" @click.native="modals.classic = true">
            View Platform
        </n-button>
    </div>
    

    <!-- Classic Modal -->
    <modal :show.sync="modals.classic" headerClasses="justify-content-center">
      <h4 slot="header" class="title title-up">Modal title</h4>
      <p>
        Far far away, behind the word mountains, far from the countries Vokalia
        and Consonantia, there live the blind texts. Separated they live in
        Bookmarksgrove right at the coast of the Semantics, a large language
        ocean. A small river named Duden flows by their place and supplies it
        with the necessary regelialia. It is a paradisematic country, in which
        roasted parts of sentences fly into your mouth.
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
  }
}
</script>
<style lang="scss" scoped>
    
</style>