<template>
  <header style="position:relative">
    <!-- <base-nav class="navbar-main" transparent type="default" effect="dark" expand> -->
    <base-nav transparent type effect="dark" expand>
      <router-link slot="brand" class="mr-lg-5" to="/">
        <h2 class="navbar-brand">Magic App</h2>
      </router-link>

      <div class="row" slot="content-header" slot-scope="{closeMenu}">
        <div class="col-6 collapse-brand">
          <a href="../index.html">
            <!-- <img src="img/brand/blue.png" /> -->
            <h2 class="navbar-brand text-primary">Magic App</h2>
          </a>
        </div>
        <div class="col-6 collapse-close">
          <close-button @click="closeMenu"></close-button>
        </div>
      </div>

      <ul class="navbar-nav navbar-nav-hover ml-lg-auto">
        <li class="nav-item">
          <!-- <a class="nav-link"> -->
          <router-link class="nav-link" to="/">
            <i class="ni ni-ui-04 d-lg-none"></i>
            <span class="nav-link-inner--text">Home</span>
          </router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" to="/about-us">
            <i class="ni ni-ui-04 d-lg-none"></i>
            <span class="nav-link-inner--text">About Us</span>
          </router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" to="/how-it-works">
            <i class="ni ni-ui-04 d-lg-none"></i>
            <span class="nav-link-inner--text">How It Works</span>
          </router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" to="/how-it-works">
            <i class="ni ni-ui-04 d-lg-none"></i>
            <span class="nav-link-inner--text">Pricing</span>
          </router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" to="/how-it-works">
            <i class="ni ni-ui-04 d-lg-none"></i>
            <span class="nav-link-inner--text">Download the App</span>
          </router-link>
        </li>
        <li class="nav-item dropdown">
          <a href class="nav-link" data-toggle="dropdown" role="button">
            <i class="ni ni-collection d-lg-none"></i>
            <span class="nav-link-inner--text">More</span>
          </a>
          <div class="dropdown-menu">
            <router-link to="/landing" class="dropdown-item">Blog</router-link>
            <router-link to="/profile" class="dropdown-item">Contact</router-link>
            <router-link to="/login" class="dropdown-item">T&C's</router-link>
          </div>
        </li>
      </ul>
    </base-nav>
  </header>
</template>
<script>
import BaseNav from "@/components/BaseNav";
import CloseButton from "@/components/CloseButton";

export default {
  components: {
    BaseNav,
    CloseButton
  }
};
</script>
<style>
</style>
