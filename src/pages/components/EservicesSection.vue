<template>
    <div class="section section-basic">
      <div class="">
          <div class="col-md-6 ml-auto mr-auto">
              <h2 class="title text-center">Our Services</h2>
          </div>
          <tabs
              pills
              class="nav-align-center"
              tab-content-classes="gallery"
              tab-nav-classes="nav-pills-just-icons"
              type="primary"
          >
              <tab-pane title="Development">
                  <i slot="label" class="now-ui-icons design_app"></i>
                  <div class="col-md-10 ml-auto mr-auto">
                      <div class="section section-nucleo-icons">
                        <div class="container">

                          <div class="row justify-content-md-center">
                            <div class="text-center col-md-12 col-lg-8">
                              <h3 class="title">IT Products and Services</h3>
                              <h5 class="description">
                                MISA eServices offers IT Consultancy so we can improve your organization by leveraging IT to your advantage. We also offer web and systems development to help you build your online presence, or to make your processes more effective and efficient to maximize your business potential.
                              </h5>
                            </div>
                            <div class="text-center col-md-12 col-lg-8">
                              <a
                                href="/contact"
                                class="btn btn-primary btn-lg btn-round"
                                role="button"
                              >
                                Contact Us
                              </a>
                              <a
                                href="/development-services"
                                class="btn btn-primary btn-lg btn-simple btn-round"
                                role="button"
                              >
                                Learn More
                              </a>
                            </div>
                          </div>

                        </div>
                      </div>
                  </div>
              </tab-pane>

              <tab-pane title="Workshops">
                  <i slot="label" class="now-ui-icons education_hat"></i>
                  <div class="col-md-10 ml-auto mr-auto">
                      <div class="section section-nucleo-icons">
                        <div class="container">
                          <div class="row justify-content-md-center">
                            <div class="text-center col-md-12 col-lg-8">
                              <h3 class="title">Development Workshops</h3>
                              <h5 class="description">
                                placeholder text
                              </h5>
                            </div>
                            <div class="text-center col-md-12 col-lg-8">
                              <a
                                href="/workshops"
                                class="btn btn-primary btn-lg btn-round"
                                role="button"
                              >
                                Workshops Schedule
                              </a>
                            </div>
                          </div>
                          

                        </div>
                      </div>
                  </div>
              </tab-pane>

              <tab-pane title="Helpdesk">
                  <i slot="label" class="now-ui-icons emoticons_satisfied"></i>
                  <div class="col-md-10 ml-auto mr-auto">
                      <div class="section section-nucleo-icons">
                        <div class="container">
                          <div class="row justify-content-md-center">
                            <div class="text-center col-md-12 col-lg-8">
                              <h3 class="title">eServices Helpdesk</h3>
                              <h5 class="description">
                                placeholder text
                              </h5>
                            </div>
                            <div class="text-center col-md-12 col-lg-8">
                              <a
                                href="/helpdesk"
                                class="btn btn-primary btn-lg btn-round"
                                role="button"
                              >
                                Contact Us
                              </a>
                              <a
                                href="/development"
                                class="btn btn-primary btn-lg btn-simple btn-round"
                                role="button"
                              >
                                About Helpdesk
                              </a>
                            </div>
                          </div>
                        </div>
                      </div>
                  </div>
              </tab-pane>
          </tabs>
      </div>
    </div>
</template>
<script>
import { Tabs, TabPane } from '@/components';



export default {
  name: 'EservicesSection',
  bodyClass: 'index-page',
  components: {
    Tabs,
    TabPane
  }
};
</script>
<style lang="scss" scoped>
.description{
    color: #2c2c2c;
}
</style>
