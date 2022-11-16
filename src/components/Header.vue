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
  <div class="header h-20 w-full bg-red-400 flex flex-row">
    <Hamburger />
    <h2 class="text-primary text-2xl font-body">TUNIFY</h2>
    <div class="search__section">
      <input type="text" />
    </div>
    <div class="user__section">
      <Notification />
      <Cog />
    </div>
  </div>
</template>
