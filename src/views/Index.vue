<template>
  <div class="home">
    <Navbar />
    <HeroSection />
    <Intro />
    <Features />
    <Products />
    <Partners />
    <Banner />
    <Footer />
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue';
import HeroSection from '@/components/HeroSection.vue';
import Intro from '@/components/Intro.vue';
import Products from '@/components/Products.vue';
import Partners from '@/components/Partners.vue';
import Banner from '@/components/Banner.vue';
import Footer from '@/components/Footer.vue';
import Features from '@/components/Features.vue';
export default {
  components:{
    Navbar,
    HeroSection,
    Intro,
    Features,
    Products,
    Partners,
    Banner,
    Footer
  }
}
</script>
