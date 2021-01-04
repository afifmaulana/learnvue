<template>
  <div id="app">
    <Navbar/>
    <div class="relativebg-white antialiased overflow-hidden">
        <div class="max-w-7xl mx-auto">
            <div class="relative z-10 pb-8 sm:pb-16 md:pb-20 lg:max-w-2xl lg:w-full lg:pb-28 xl:pb-32">
                <Main/>
            </div>
        </div>
        <div class="lg:absolute lg:inset-y-0 lg:right-0 lg:w-1/2">
            <img class="h-56 w-full object-cover sm:h-72 md:h-96 py-14 px-4 lg:w-full lg:h-full" src="images/banner.jpg" alt="">
          </div>

    </div>
    <Gallery/>
    <Footer/>
    <router-view/>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Main from './components/Main.vue'
import Gallery from './components/Gallery.vue'
import Footer from './components/Footer.vue'
export default {
  components : {
    Navbar,
    Gallery,
    Footer,
    Main
  }
}
</script>
