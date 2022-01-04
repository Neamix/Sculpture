<template>
  <div class="container bg-silver-1000 min-h-screen	min-w-full">
      <Navbar/>
      <Header/>
      <LowerNav/>
  </div>
</template>

<style>

body {
    @apply bg-silver-1000;
}

#app {
  font-family: 'PT Sans';
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

.drop-menu {
  top: 39px;
  left: 0;
  @apply absolute; 
  @apply w-full; 
  @apply bg-silver-1000; 
  @apply rounded-md p-2
}

/** 
Animated classes
*/

.slide-enter-active,
.slide-leave-active {
  transition: all .3s linear;
}

.slide-enter-to,
.slide-leave-from {
  opacity: 1;
  top: 39px;
}

.slide-leave-to,
.slide-enter-from {
  opacity: 0;
  top: 55px;
}

</style>

<script>
import Header from '@/components/Header.vue'
import Navbar from '@/components/Navbar.vue'
import LowerNav from '@/components/LowerNav.vue'

export default ({
  components: {
    Header,
    Navbar,
    LowerNav
   }
})
</script>

