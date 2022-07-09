<template>
  <div class="nes-container with-title mb-10">
    <p class="title">Soldiers of Valhalla NFT</p>
    <p>Welcome to Soldiers of Valhalla NFT STAKING app !</p>
    <p class="mt-5">
      You can stake your VIKING NFT here.
    </p>
     <p class="mt-5">
      Note: Staking fees are and rewards claiming fees are up paid by the staker.
    </p>
    <p class="mt-5">
      Gem Farm is deployed at:
      <span class="bg-yellow-100">{{ DEFAULTS.GEM_FARM_PROG_ID }}</span>
    </p>
  </div>
    <div class="nes-container mb-10 ">
      <video class="m-auto" autoPlay={true} loop={true} muted src='../assets/sov.mp4'>
      </video>
  </div>
  <div class="flex flex-row">
    <div class="nes-container with-title flex-1 ">
      <p class="title">Stake your NFTs</p>
      <p class="mb-5">
        Stake your soldiers here!
      </p>
      <router-link to="staking">
        <button class="md-btn md-bg-indigo-900 md-color-white ripple-surface"><p>Here</p></button>
      </router-link>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { DEFAULTS } from '@/globals';
export default defineComponent({
  setup() {
    return {
      DEFAULTS,
    };
  },
});
</script>
<style scoped></style>
