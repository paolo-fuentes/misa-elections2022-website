<template>
  <navbar
    position="fixed"
    type="primary"
    :transparent="transparent"
    :color-on-scroll="colorOnScroll"
    menu-classes="ml-auto"
  >
    <template>
      <router-link v-popover:popover1 class="navbar-brand" to="/">
        <img class="" src="img/now-logo.png" alt="" style="height: 42px; width: 42px;"/>
      </router-link>
      
    </template>
    <template slot="navbar-menu">
      <li class="nav-item">
        <a
          class="nav-link"
          href="#/"
        >
          <p>Home</p>
        </a>
      </li>

      <li class="nav-item">
        <a
          class="nav-link"
          href="#/about"
        >
          <p>About</p>
        </a>
      </li>

      <drop-down
              tag="li"
              title="Services"
              class="nav-item"
      >
        <nav-link to="/development-services">
          <i class="now-ui-icons design_app"></i> IT Products and Services
        </nav-link>
        <nav-link to="/workshops">
          <i class="now-ui-icons education_hat"></i> Development Workshops
        </nav-link>
        <nav-link to="/helpdesk">
          <i class="now-ui-icons emoticons_satisfied"></i> eServices Helpdesk
        </nav-link>
      </drop-down>

      <li class="nav-item">
        <a
          class="nav-link"
          href="#/contact"
        >
          <p>Contact Us</p>
        </a>
      </li>
    </template>
  </navbar>
</template>

<script>
import { DropDown, Navbar, NavLink } from '@/components';
import { Popover } from 'element-ui';
export default {
  name: 'main-navbar',
  props: {
    transparent: Boolean,
    colorOnScroll: Number
  },
  components: {
    Navbar,
    NavLink,
    DropDown,
    [Popover.name]: Popover
  }
};
</script>

<style scoped></style>
