<script>
// import { Icon } from "@iconify/vue";
import Hamburger from "./icons/Hamburger.vue";
import Notification from "./icons/Notification.vue";
import Cog from "./icons/Cog.vue";

export default {
  name: "Header",
  components: {
    Hamburger,
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
      <div class="search__section font-body">
        <input type="text" placeholder="Search for songs,.." />
      </div>
      <div class="user__section flex items-center gap-3">
        <Notification class="w-5" />
        <Cog class="w-5" />
        <span class="user__image w-5 h-5 bg-primary rounded-full"></span>
      </div>
    </div>
  </header>
</template>
