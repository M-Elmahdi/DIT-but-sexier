<template>

<div>
    <!-- Spinner Start -->
    <div
      id="spinner"
      class="bg-white position-fixed translate-middle w-100 vh-100 top-50 start-50 d-flex align-items-center justify-content-center"
      :class="isLoading ? 'show' : ''"
    >
      <div class="spinner-grow text-primary" role="status"></div>
    </div>
    <!-- Spinner End -->
    
    <!-- Topbar Start -->
    <top-bar :lang="lang" />
    <!-- Topbar End -->

    <!-- English Components -->
    <div v-if="selectedLang === 'en'">
      <!-- Navbar Start -->
      <en-navbar @changeLang="changeLang()" :lang="lang" />
      <!-- Navbar End -->

      <!-- Carousel Start -->
      <en-carousel :lang="lang" />
      <!-- Carousel End -->

      <!-- About Start -->
      <en-about :lang="lang" />
      <!-- About End -->

      <!-- Vision Start -->
      <en-vision :lang="lang" />
      <!-- Vision End -->

      <!-- Features Start -->
      <en-features :lang="lang" />
      <!-- Features End -->

      <!-- Service Start -->
      <en-services :lang="lang" />
      <!-- Service End -->

      <!-- Appointment Start -->
      <en-appointment :lang="lang" />
      <!-- Appointment End -->

      <!-- Twitter Feed -->
      <en-blog :lang="lang"/>
      <!-- End Twitter Feed-->

      <!-- Footer Start -->
      <en-footer :lang="lang" />
      <!-- Footer End -->
    </div>
    <!-- End English Components -->


    <!-- Arabic Components -->
    <div class="hacen-regular" v-else>
      <!-- Navbar Start -->
      <ar-navbar @changeLang="changeLang()" :lang="lang" />
      <!-- Navbar End -->

      <!-- Carousel Start -->
      <ar-carousel :lang="lang" />
      <!-- Carousel End -->

      <!-- About Start -->
      <ar-about :lang="lang" />
      <!-- About End -->

      <!-- Vision Start -->
      <ar-vision :lang="lang" />
      <!-- Vision End -->

      <!-- Features Start -->
      <ar-features :lang="lang" />
      <!-- Features End -->

      <!-- Service Start -->
      <ar-services :lang="lang" />
      <!-- Service End -->

      <!-- Appointment Start -->
      <ar-appointment :lang="lang" />
      <!-- Appointment End -->

      <!-- Twitter Feed -->
      <ar-blog :lang="lang"/>
      <!-- End Twitter Feed-->

      <!-- Footer Start -->
      <ar-footer :lang="lang" />
      <!-- Footer End -->
    </div>
    <!-- End Arabic Components -->


    <!-- Back to Top -->
    <a href="#" class="btn btn-lg btn-primary btn-lg-square back-to-top">
      <i class="bi bi-arrow-up"></i>
    </a>
</div>
  
</template>

<script>
/**
 * 
 * Language Importing
 * 
 * */

import enLang from '@/lang/en';
import arLang from '@/lang/ar';

/**
 * 
 * End Language Importing
 * 
 * */

/**
 * 
 * English Components
 * 
 * */
import TopBar from '@/components/unified/TopBar.vue'
import EnNavbar from '@/components/en/Navbar.vue';
import EnCarousel from '@/components/en/Carousel.vue';
import EnAbout from '@/components/en/About.vue';
import EnVision from '@/components/en/Vision.vue';
import EnFooter from '@/components/en/Footer.vue';
import EnAppointment from '@/components/en/Appointment.vue';
import EnServices from '@/components/en/Services.vue';
import EnFeatures from '@/components/en/Features.vue';
import EnBlog from '@/components/en/Blog.vue';


/**
 * 
 * Arabic Components
 * 
 * */
import ArNavbar from '@/components/ar/Navbar.vue';
import ArCarousel from '@/components/ar/Carousel.vue';
import ArAbout from '@/components/ar/About.vue';
import ArVision from '@/components/ar/Vision.vue';
import ArFooter from '@/components/ar/Footer.vue';
import ArAppointment from '@/components/ar/Appointment.vue';
import ArServices from '@/components/ar/Services.vue';
import ArFeatures from '@/components/ar/Features.vue';
import ArBlog from '@/components/ar/Blog.vue';

export default {
  name: 'App',
  components: {
    TopBar,
    // English Components
    EnNavbar, EnCarousel, EnAbout, EnVision, EnFooter, EnAppointment, EnServices, EnFeatures, EnBlog,

    // Arabic Components
    ArNavbar, ArCarousel, ArAbout, ArVision, ArFooter, ArAppointment, ArServices, ArFeatures, ArBlog
  },   

  data(){
    return {
      selectedLang: 'en',
      lang: enLang,
      isLoading: true,
    }
  },
  methods: {
    changeLang(){
      if (this.selectedLang === 'en') {
        this.selectedLang = 'ar';
        this.lang = arLang;
      } else {
        this.selectedLang = 'en';
        this.lang = enLang;
      }
    }
  },
  mounted(){
      setTimeout(() => {
        this.isLoading = false
      }, 3000);
  },
}
</script>

