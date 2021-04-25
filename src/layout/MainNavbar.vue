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

      <li class="nav-item">
        <a
          class="nav-link"
          href="#/"
        >
          <p>Services</p>
        </a>
      </li>

      <li class="nav-item">
        <a
          class="nav-link"
          href="#/"
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
    [Popover.name]: Popover
  }
};
</script>

<style scoped></style>
