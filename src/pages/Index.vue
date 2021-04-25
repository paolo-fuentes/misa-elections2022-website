<template>
  <div>
    <div class="page-header clear-filter" filter-color="orange">
      <parallax
        class="page-header-image"
        style="background-image:url('img/header.jpg')"
      >
      </parallax>
      <div class="container">
        <div class="content-center brand">
          <img class="n-logo" src="img/now-logo.png" alt="" />
          <h1 class="h1-seo">eServices</h1>
          <h3>Ateneo Management Information Systems Association</h3>
        </div>
      </div>
    </div>
    <div class="main">
      <div class="section section-images">
        <div class="container">
          <div class="row">
            <div class="col-md-12">
              <div class="hero-images-container">
                <img src="img/hero-image-1.png" alt="" />
              </div>
              <div class="hero-images-container-1">
                <img src="img/hero-image-2.png" alt="" />
              </div>
              <div class="hero-images-container-2">
                <img src="img/hero-image-3.png" alt="" />
              </div>
            </div>
          </div>
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
            <a
              href="#/about"
              class="btn btn-primary btn-lg btn-simple btn-round"
              role="button"
            >
              Learn More
            </a>
          </div>
        </div>
        <div class="separator separator-primary"></div>
        <div class="section-story-overview">
          <div class="row">
            <div class="col-md-6">
              <div
                class="image-container image-left"
                style="background-image: url('img/login.jpg')"
              >
                <!-- First image on the left side -->
                <p class="blockquote blockquote-primary">
                  "The next step to business technology"
                  <br />
                  <br />
                  <!-- <small>-MISA</small> -->
                </p>
              </div>
              <!-- Second image on the left side of the article -->
              <div
                class="image-container"
                style="background-image: url('img/bg3.jpg')"
              ></div>
            </div>
            <div class="col-md-5">
              <!-- First image on the right side, above the article -->
              <div
                class="image-container image-right"
                style="background-image: url('img/bg1.jpg')"
              ></div>
              <h3>
                The next step to business technology.
              </h3>
              <p>
                The Arctic Ocean freezes every winter and much of the sea-ice
                then thaws every summer, and that process will continue whatever
                happens with climate change. Even if the Arctic continues to be
                one of the fastest-warming regions of the world, it will always
                be plunged into bitterly cold polar dark every winter. And
                year-by-year, for all kinds of natural reasons, there’s huge
                variety of the state of the ice.
              </p>
              <p>
                For a start, it does not automatically follow that a record
                amount of ice will melt this summer. More important for
                determining the size of the annual thaw is the state of the
                weather as the midnight sun approaches and temperatures rise.
                But over the more than 30 years of satellite records, scientists
                have observed a clear pattern of decline, decade-by-decade.
              </p>
              <p>
                The Arctic Ocean freezes every winter and much of the sea-ice
                then thaws every summer, and that process will continue whatever
                happens with climate change. Even if the Arctic continues to be
                one of the fastest-warming regions of the world, it will always
                be plunged into bitterly cold polar dark every winter. And
                year-by-year, for all kinds of natural reasons, there’s huge
                variety of the state of the ice.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    
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
                                <h3 class="title">Systems Design and Development</h3>
                                <h5 class="description">
                                  MISA eServices offers IT Consultancy so we can improve your organization by leveraging IT to your advantage. We also offer web and systems development to help you build your online presence, or to make your processes more effective and efficient to maximize your business potential.
                                </h5>
                              </div>
                              <div class="text-center col-md-12 col-lg-8">
                                <a
                                  href="#/contact"
                                  class="btn btn-primary btn-lg btn-round"
                                  role="button"
                                >
                                  Contact Us
                                </a>
                                <a
                                  href="#/development"
                                  target="_blank"
                                  class="btn btn-primary btn-lg btn-simple btn-round"
                                  role="button"
                                >
                                  Our Process
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
                                <h3 class="title">Workshops</h3>
                                <h5 class="description">
                                  MISA eServices offers IT Consultancy so we can improve your organization by leveraging IT to your advantage. We also offer web and systems development to help you build your online presence, or to make your processes more effective and efficient to maximize your business potential.
                                </h5>
                              </div>
                              <div class="text-center col-md-12 col-lg-8">
                                <a
                                  href="#/contact"
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
                                  MISA eServices offers IT Consultancy so we can improve your organization by leveraging IT to your advantage. We also offer web and systems development to help you build your online presence, or to make your processes more effective and efficient to maximize your business potential.
                                </h5>
                              </div>
                              <div class="text-center col-md-12 col-lg-8">
                                <a
                                  href="#/contact"
                                  class="btn btn-primary btn-lg btn-round"
                                  role="button"
                                >
                                  Contact Us
                                </a>
                                <a
                                  href="#/development"
                                  target="_blank"
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


  </div>
</template>
<script>
import { Parallax, Tabs, TabPane } from '@/components';



export default {
  name: 'index',
  bodyClass: 'index-page',
  components: {
    Parallax,
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
