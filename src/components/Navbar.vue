<template>
    <div class="pl-10 pt-5 flex absolute w-full z-10">
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
                <input class="input rounded-full p-1.5 text-sm pl-4  text-white outline-none bg-gray-1000 w-full" type="search" placeholder="Search...">
                </form>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>
