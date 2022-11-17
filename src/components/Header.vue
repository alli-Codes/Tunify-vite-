<script>
// import { Icon } from "@iconify/vue";
import Hamburger from "./icons/Hamburger.vue";
import Search from "./icons/Search.vue";
import Notification from "./icons/Notification.vue";
import Cog from "./icons/Cog.vue";

export default {
  name: "Header",
  components: {
    Hamburger,
    Search,
    Notification,
    Cog,
  },
};
</script>

<template>
  <header class="w-full px-4 flex justify-center">
    <div class="h-20 w-full flex justify-between items-center gap-4">
      <div class="flex items-center gap-4">
        <Hamburger class="w-5" />
        <h2 class="text-primary text-2xl font-body">T</h2>
      </div>
      <div
        class="search__section w-full md:max-w-[24rem] lg:max-w-[32rem] h-8 bg-green-400 flex font-body border border-primary rounded-sm relative"
      >
        <Search class="w-5 z-10" />
        <input
          type="text"
          class="h-full w-full pl-9 pr-3 py-2 outline-0 absolute"
          placeholder="Search for songs,.."
        />
      </div>
      <div
        class="user__section bg-red-400 flex justify-end items-center gap-3 md:gap-6"
      >
        <Notification class="w-5" />
        <Cog class="w-5" />
        <div class="user__details flex">
          <span class="user__image w-5 h-5 bg-primary rounded-full"></span>
          <p class="user__name hidden md:flex">Ademola Michael</p>
        </div>
      </div>
    </div>
  </header>
</template>
