<script>
import HomeIcon from "./icons/HomeIcon.vue";
import ExploreIcon from "./icons/ExploreIcon.vue";
import SongsIcon from "./icons/SongsIcon.vue";
import ArtistIcon from "./icons/ArtistIcon.vue";
import AlbumIcon from "./icons/AlbumIcon.vue";
import RadioIcon from "./icons/RadioIcon.vue";
import RecentIcon from "./icons/RecentIcon.vue";
import FavoriteIcon from "./icons/FavoriteIcon.vue";
import PlaylistIcon from "./icons/PlaylistIcon.vue";

export default {
  name: "Sidebar",
  components: {
    HomeIcon,
    ExploreIcon,
    SongsIcon,
    ArtistIcon,
    AlbumIcon,
    RadioIcon,
    RecentIcon,
    FavoriteIcon,
    PlaylistIcon,
  },
  data() {
    return {
      activeColor: "#00D38B",
    };
  },
};
</script>

<template>
  <div class="h-full w-[20rem] bg-[#FFF8F8] absolute top-0">
    <div class="bg-red-40 font-body flex flex-col relative top-20">
      <section class="pt-10 flex flex-col gap-10">
        <p class="px-5 text-[#C4C4C4] text-[10px]">BROWSER</p>
        <nav class="bg-green-40 flex flex-col gap-4 text-xs">
          <a href="#"><HomeIcon class="w-4" />Home</a>
          <a href="#" class="active"
            ><ExploreIcon class="w-4" :activeColor="activeColor" />Explore</a
          >
          <a href="#"><SongsIcon class="w-4" /> Songs</a>
          <a href="#"><ArtistIcon class="w-4" />Artists</a>
          <a href="#"><AlbumIcon class="w-4" />Albums</a>
          <a href="#"><RadioIcon class="w-4" />Radio</a>
        </nav>
      </section>

      <section class="pt-10 flex flex-col gap-10">
        <p class="px-5 text-[#C4C4C4] text-[10px]">YOUR LIBRARY</p>
        <nav class="bg-green-40 flex flex-col gap-4 text-xs">
          <a href="#"><RecentIcon class="w-4" />Recently Played</a>
          <a href="#"><FavoriteIcon class="w-4" />Favourites</a>
          <a href="#"><PlaylistIcon class="w-4" />Playlists</a>
        </nav>
      </section>

      <section class="pt-10 pl-6 flex flex-col gap-8">
        <img src="/images/g-store-light.png" class="w-32" alt="" />
        <img src="/images/a-store-light.png" class="w-32" alt="" />
      </section>
    </div>
  </div>
</template>

<style scoped>
nav a {
  width: 100%;
  padding: 0.5rem 1rem;
  border-left: 5px solid transparent;
  font-weight: bold;
  display: flex;
  gap: 0.5rem;
}

nav .active {
  background-color: #fff8f8;
  border-left: 5px solid #00d38b;
}
</style>
