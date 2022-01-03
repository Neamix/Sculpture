<template>
  <div class="container bg-silver-1000 min-h-screen	min-w-full">
      <Navbar/>
      <Header/>
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

