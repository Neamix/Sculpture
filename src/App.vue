<template>
  <div class="container bg-silver-1000 min-h-screen	min-w-full">
      <Header/>
      <Navbar/>
      <header class="w-full min-h-screen flex items-center relative">
         <div class="p-10 relative z-10">
            <h2 class="text-white font-bold w-1/2">Sia Career Life</h2>
            <div class="podcast-stars flex text-white mt-2 mb-2">
               <i class="ri-star-fill"></i>
               <i class="ri-star-fill pl-2"></i>
               <i class="ri-star-fill pl-2"></i>
               <i class="ri-star-fill pl-2"></i>
               <i class="ri-star-line pl-2"></i>
            </div>
            <p class="text-sm w-1/2 text-white">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged</p>
            <button class="btn relative flex">
              <i class="ri-headphone-line z-10 pr-2"></i>
              <p class="z-10">Listen Podcast</p>
            </button>
         </div>
         <div class="overlay w-full h-full "></div>
      </header>
  </div>
</template>

<style>

body {
    @apply bg-silver-1000;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}



header {
  background: url('assets/images/vintage-old-rustic-cutlery-dark.jpg');
  background-size: cover;
}

header .overlay {
  @apply bg-silver-1000; 
  @apply absolute;
  top: 0;
  opacity: 0.5;
}

header::before {
  content:'';
  height: 45px;
  @apply w-full;
    content: '';
    height: 387px;
    background: linear-gradient(358deg, black, black ,transparent);
    width: 100%;
    display: block;
    position: absolute;
    bottom: 0;
}

header h2 {
  font-size: 50px;
  width: 64%;
}

.btn {
  @apply text-white;
  @apply rounded-md ;
  @apply bg-silver-1000 rounded-l-sm;
  @apply p-2 ;
  @apply text-sm;  
  @apply pl-4  ;
  @apply pr-4 ;
  @apply mt-5 ;
  @apply outline-none ;
  transition: all .5s linear;
}

.btn::before {
  content: '';
  display: block;
  @apply bg-black;
  @apply rounded-r-md;
  @apply bg-silver-900;
  @apply rounded-l-sm;
  height: 100%;
  position: absolute;
  bottom: 0;
  left: 0;
  transition: all .2s linear;
  width: 0%;
}

.btn:hover::before {
    width: 50%;
}

</style>

<script>
import Header from '@/components/Header.vue'
import Navbar from '@/components/Navbar.vue'

export default ({
  components: {
    Header,
    Navbar
   }
})
</script>

