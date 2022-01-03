<template>
    <div class="pl-10 pt-5  absolute w-full z-10 flex lg:hidden">
        <div class="logo"></div>
        <ul class="flex">
            <li class="menu-item">
                <router-link to="#" class="text-white text-sm pl-2">Discover</router-link>
            </li>
            <li class="menu-item">
                <router-link to="#" class="text-white text-sm pl-2">Browse</router-link>
            </li>
            <li class="menu-item">
                <router-link to="#" class="text-white text-sm pl-2">Your Library</router-link>
            </li>
        </ul>
        <ul class="flex ml-auto mr-5 w-7/12">
            <li class="menu-item w-5/12">
                <form>
                    <i class="ri-search-line absolute search-icon text-xs text-white"></i>
                    <input class="input rounded-full p-1.5 text-sm pl-8 text-white outline-none bg-gray-1000 w-full" type="search" placeholder="Search...">
                </form>
            </li>
            <li class="menu-item ml-auto user_tab flex  items-center">
                <img src="../assets/images/users_images/user1.jpg" alt="Abdalrhman Hussin" class="profile_image rounded-full" />
                <span class="text-white text-xs font-bold ml-2">Abdalrhman Hussin</span>
                <i class="ri-arrow-down-s-line pl-2 text-white"></i>
            </li>
            <li class="menu-item">
                <form class="relative">
                    <i class="ri-search-line absolute search-icon text-xs text-white"></i>
                    <input class="input rounded-full p-1.5 text-sm pl-8 text-white outline-none bg-gray-1000 w-full" type="search" placeholder="Search...">
                    <ul class="menu-result absolute drop-menu bg-silver-1000 w-full" v-if="dropDownSearch">
                        <li class="menu-item">
                            <router-link to="#">
                                <div class="result mt-1">
                                    <p class="text-sm text-white">How to be reach in short time</p>
                                    <p class="text-sm text-whity">Auther: <span>Adam Jacob</span></p>
                                </div>
                            </router-link>
                        </li>
                        <li class="menu-item">
                            <router-link to="#">
                                <div class="result mt-2">
                                    <p class="text-sm text-white">How to be reach in short time</p>
                                    <p class="text-sm text-whity">Auther: <span>Adam Jacob</span></p>
                                </div>
                            </router-link>
                        </li>
                        <li class="menu-item">
                            <router-link to="#">
                                <div class="result mt-2">
                                    <p class="text-sm text-white">How to be reach in short time</p>
                                    <p class="text-sm text-whity">Auther: <span>Adam Jacob</span></p>
                                </div>
                            </router-link>
                        </li>
                        <li class="menu-item">
                            <router-link to="#">
                                <div class="result mt-2">
                                    <p class="text-sm text-white">How to be reach in short time</p>
                                    <p class="text-sm text-whity">Auther: <span>Adam Jacob</span></p>
                                </div>
                            </router-link>
                        </li>
                        <li class="menu-item">
                            <router-link to="#">
                                <div class="result mt-2">
                                    <p class="text-sm text-white">How to be reach in short time</p>
                                    <p class="text-sm text-whity">Auther: <span>Adam Jacob</span></p>
                                </div>
                            </router-link>
                        </li>
                    </ul>
                </form>
            </li>
            <li class="menu-item ml-auto user_tab flex  items-center relative">
                <img src="../assets/images/users_images/user1.jpg" alt="Abdalrhman Hussin" class="profile_image rounded-full" />
                <span class="text-white text-xs font-bold ml-2">Abdalrhman Hussin</span>
                <i class="ri-arrow-down-s-line pl-2 text-white"></i>
                <ul class="drop-menu" v-if="dropDownProfile">
                    <li class="menu-item text-white text-sm flex">
                        <i class="ri-map-pin-user-line mr-3"></i>
                        Profile
                    </li>
                    <li class="menu-item text-white text-sm pt-2">
                        <i class="ri-settings-5-fill mr-3"></i>
                        Settings
                    </li>
                </ul>
            </li>
        </ul>
    </div>
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
    
</style>

<script>
export default {
  name: 'Navbar',
  data() {
    return {
        dropDownProfile: false,
        dropDownSearch: false,
        searchResultArray: []
    }
  },

  methods: {

  }
}
</script>
