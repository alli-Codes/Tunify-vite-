<script></script>

<template>
  <div class="h-full w-[20rem] bg-[#FFF8F8] absolute top-0">
    <div class="bg-red-40 font-body flex flex-col relative top-20">
      <section class="pt-10 flex flex-col gap-10">
        <p class="px-5 text-[#C4C4C4]">BROWSER</p>
        <nav class="bg-green-40 flex flex-col gap-4">
          <a href="#">Home</a>
          <a href="#" class="active">Explore</a>
          <a href="#">Songs</a>
          <a href="#">Artists</a>
          <a href="#">Albums</a>
          <a href="#">Radio</a>
        </nav>
      </section>

      <section class="pt-10 flex flex-col gap-10">
        <p class="px-5 text-[#C4C4C4]">YOUR LIBRARY</p>
        <nav class="bg-green-40 flex flex-col gap-4">
          <a href="#">Recently Played</a>
          <a href="#">Favourites</a>
          <a href="#">Playlists</a>
        </nav>
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
}

nav .active {
  background-color: #fff8f8;
  border-left: 5px solid #00d38b;
}
</style>
