<template>
    <header class="w-full min-h-screen flex items-center relative">
         <div class="p-10 relative z-10">
            <h2 class="text-white font-bold w-1/2 sm:w-full text-head sm:text-3xl">Sia Career Life</h2>
            <div class="podcast-stars flex text-white mt-2 mb-2">
               <i class="ri-star-fill"></i>
               <i class="ri-star-fill pl-2"></i>
               <i class="ri-star-fill pl-2"></i>
               <i class="ri-star-fill pl-2"></i>
               <i class="ri-star-line pl-2"></i>
            </div>
            <p class="text-sm w-1/2 text-white sm:w-full">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged</p>
            <button class="btn relative flex">
              <i class="ri-headphone-line z-10"></i>
              <p class="z-10 ml-2">Listen Podcast</p>
            </button>
         </div>
         <div class="overlay w-full h-full "></div>
    </header>
</template>

<style scoped>
    form .search-icon {        
        padding: 9px 8px;
        color: #A0AEA2;
    }

    .user_tab {
        height: fit-content;
        @apply bg-silver-1000;
        padding: 3px 8px;
        border-radius: 200px;
    }

    .user_tab .profile_image {
        width: 20px;
        height: 20px;
    }

    .user_tab span {
        font-size: 11px;
    }
    
    header {
        background: url('../assets/images/vintage-old-rustic-cutlery-dark.jpg');
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
  @apply w-full;
  height: 387px;
  background: linear-gradient(358deg, black, black ,transparent);
  width: 100%;
  display: block;
  position: absolute;
  bottom: 0;
}

header h2 {
  width: 64%;
}
</style>