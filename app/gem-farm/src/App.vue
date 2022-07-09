<template>
  <div class="relative h-full min-h-screen bg_container"
   
  >
    <TheNavBar />
    <div class="pt-10 px-10 flex justify-center align-middle"
    >
      <p class="text-4xl pt-3 px-1 mt-1 text-black">Soldiers of Valhalla NFT</p>
      <img :width="50" :height="50" src="./assets/V.png" />
    </div>

    <div class="p-10">
      <router-view />
    </div>

    <div class="pt-10"></div>
    <TheFooter />
  </div>
</template>

<script>
import TheNavBar from '@/components/TheNavBar';
import TheFooter from '@/components/gem-farm/TheFooter';
export default {
  components: { TheFooter, TheNavBar },
  data() {
    return {
      image: "./assets/odin.png",
    };
  }
};
</script>

<style>
* {
  font-family: 'VIKING', monospace;
}

input[type='radio']:checked + span {
  @apply text-black;
}
</style>
