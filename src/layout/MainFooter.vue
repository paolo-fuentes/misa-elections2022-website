<template>
  <footer
    class="footer"
    :class="{ [`footer-${type}`]: type }"
    :data-background-color="backgroundColor"
  >
    <div class="container">
      <nav>
        <ul>
          <li>
            <a href="#/">
              Home
            </a>
          </li>
          <li>
            <a href="#/about">
              About
            </a>
          </li>
          <li>
            <a href="#/development-services">
              Development
            </a>
          </li>
          <li>
            <a href="#/workshops">
              Workshops
            </a>
          </li>
          <li>
            <a href="#/helpdesk">
              Helpdesk
            </a>
          </li>
          <li>
            <a href="#/contact">
              Contact
            </a>
          </li>
        </ul>
      </nav>
      <div class="copyright">
        &copy; {{ year }}, Developed by MISA eServices
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>
<style></style>
