<template>
  <div>
    <nav>
      <div class="container">
        <a href="" class="nav-logo">
          <h3>Your Doctor</h3>
        </a>

        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#services">Services</a></li>
          <li><a href="#specialists">Specialists</a></li>
          <li><a href="#testimonials">Testimonials</a></li>
          <li><a class="btn" href="#appointment">Make Appointment</a></li>
        </ul>

        <ul class="nav-items_mobile"
            :class="this.showMobileMenu ? 'open-menu' : 'close-menu'">
          <li><a href="#">Home</a></li>
          <li><a href="#services">Services</a></li>
          <li><a href="#specialists">Specialists</a></li>
          <li><a href="#testimonials">Testimonials</a></li>
          <li><a class="btn" href="#appointment">Make Appointment</a></li>
        </ul>
        <div v-if="showMobileMenu == true">
          <button id="open_nav-btn" @click="showMenu"><box-icon name='menu' color="#ffffff"/></button>
        </div>
        <div v-if="showMobileMenu == false">
          <button id="close_nav-btn" @click="showMenu"><box-icon name='x' color="#ffffff" ></box-icon></button>
        </div>
        
      </div>
    </nav>
  </div>
</template>

<script>
import 'boxicons';

export default {
  name: 'Home',

  data() {
    return {
      showMobileMenu: true
    }
  },

  methods: {
    showMenu() {
      this.showMobileMenu = !this.showMobileMenu
    }
  }
}


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
