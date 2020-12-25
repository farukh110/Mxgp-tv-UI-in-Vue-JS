<template>

<div>
      <!-- Site Nav -->
  <nav>
    <div class="logo">
      <img width="180" src="https://www.mxgp-tv.com/assets/images/logo.svg" alt="">
    </div>
    <ul class="flex">
      <li>
        <a href="#">Home</a>
      </li>
      <li>
        <a href="#">Calender</a>
      </li>
      <li>
        <a href="#">Cat</a>
      </li>
      <li>
        <a href="#">Videos</a>
      </li>
      <li>
        <a href="#">Support</a>
      </li>
    </ul>
    <div class="right-nav-side flex">
      <a href="#">
        <i class="fas fa-user-alt"></i>
      </a>
      <button class="bg-red-600">
        Buy Now
      </button>
    </div>
    <div class="menu-mobile-icon" v-on:click="isActiveMenu = !isActiveMenu">
      <div></div>
      <div></div>
      <div></div>
    </div>
  </nav>
  <!-- /Site Nav -->

    <!-- Mobile Nav -->
  <div class="mobile-nav" v-bind:class="{close: isActiveMenu}">
    <div class="mobile-nav-header items-center justify-between">
      <ul class="flex list-none items-center justify-between mt-2">
        <li>
          <a href="#">
            <img src="https://www.mxgp-tv.com/assets/images/social/facebook.svg" alt="">
          </a>
        </li>
        <li>
          <a href="#">
            <img src="https://www.mxgp-tv.com/assets/images/social/youtube.svg" alt="">
          </a>
        </li>
        <li>
          <a href="#">
            <img src="https://www.mxgp-tv.com/assets/images/social/twitter.svg" alt="">
          </a>
        </li>

        <li>
          <a href="#">
            <img src="https://www.mxgp-tv.com/assets/images/social/instagram.svg" alt="">
          </a>
        </li>
      </ul>

      <div class="icon-cls" v-on:click="isActiveMenu = !isActiveMenu">
      </div>
    </div>
    <div class="mobile-nav-content">
      <ul>
        <li>
          <a href="#">Home</a>
        </li>
        <li>
          <a href="#">Calendar</a>
        </li>
        <li>
          <a href="#">Categories</a>
        </li>
        <li>
          <a href="#">Videos</a>
        </li>
        <li>
          <a href="#">Support</a>
        </li>
      </ul>
    </div>
    <div class="mobile-nav-footer">
      <a class="login-reg" href="#">
        <i class="fas fa-user-alt mr-3 text-xl"></i>
        Login / Register
      </a>
      <a href="#" class="buy-now">
        Buy Now
      </a>
    </div>
  </div>
  <!-- /Mobile Nav -->

  <!-- Mobile Page Header -->
  <div class="main-sec-hero mobile">
    <div class="content">
      <h1 class="lg:text-5xl md:text-4xl font-bold text-center pt-6">
        Calender
      </h1>
    </div>
  </div>
  <!-- Mobile Page Header -->

</div>

</template>

<script>

export default {

   data: () => ({ 
      
      isActiveMenu: true
      
     }),
  
  methods: {
    
    mobileMenu() {
      alert('open menu');
    }

  }

}

</script>
