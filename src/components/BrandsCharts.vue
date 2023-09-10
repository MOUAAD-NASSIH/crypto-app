<script setup>
import Bitcoin from "./icons/CoinBitcoin.vue";
import Ethereum from "./icons/CoinEthereum.vue";
import Xrp from "./icons/CoinXrp.vue";
import Ankr from "./icons/CoinAnkr.vue";
import Litecoin from "./icons/CoinLitecoin.vue";
import Solana from "./icons/CoinSolana.vue";

import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";

const currInfo = [
  {
    currency: "Bitcoin",
    image: "#",
    precentage: "+2.58%",
  },
  {
    currency: "Bitcoin",
    image: "#",
    precentage: "+2.58%",
  },
  {
    currency: "Bitcoin",
    image: "#",
    precentage: "+2.58%",
  },
];
</script>

<template>
  <section class="py-10">
    <div class="overflow-x-hidden flex items-center gap-2 md:gap-5 slider">
      <div
        class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
      >
        <Bitcoin />
        <p class="font-semibold lg:text-[18px]">Bitcoin</p>
        <button class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal">
          +2.58%
        </button>
      </div>
      <div
        class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
      >
        <Ankr />
        <p class="font-semibold lg:text-[18px]">Ankr</p>
        <button class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal">
          -2.58%
        </button>
      </div>
      <div
        class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
      >
        <Ethereum />
        <p class="font-semibold lg:text-[18px]">Ethereum</p>
        <button class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal">
          +2.58%
        </button>
      </div>
      <div
        class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
      >
        <Litecoin />
        <p class="font-semibold lg:text-[18px]">Litecoin</p>
        <button class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal">
          -2.58%
        </button>
      </div>
      <div
        class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
      >
        <Solana />
        <p class="font-semibold lg:text-[18px]">Solana</p>
        <button class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal">
          +2.58%
        </button>
      </div>
      <div
        class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
      >
        <Xrp />
        <p class="font-semibold lg:text-[18px]">Xrp</p>
        <button class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal">
          -2.58%
        </button>
      </div>
      <div
        class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
      >
        <Bitcoin />
        <p class="font-semibold lg:text-[18px]">Bitcoin</p>
        <button class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal">
          +2.58%
        </button>
      </div>
      <div
        class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
      >
        <Ankr />
        <p class="font-semibold lg:text-[18px]">Ankr</p>
        <button class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal">
          -2.58%
        </button>
      </div>
      <div
        class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
      >
        <Ethereum />
        <p class="font-semibold lg:text-[18px]">Ethereum</p>
        <button class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal">
          +2.58%
        </button>
      </div>
      <div
        class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
      >
        <Litecoin />
        <p class="font-semibold lg:text-[18px]">Litecoin</p>
        <button class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal">
          -2.58%
        </button>
      </div>
      <div
        class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
      >
        <Solana />
        <p class="font-semibold lg:text-[18px]">Solana</p>
        <button class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal">
          +2.58%
        </button>
      </div>
      <div
        class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
      >
        <Xrp />
        <p class="font-semibold lg:text-[18px]">Xrp</p>
        <button class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal">
          -2.58%
        </button>
      </div>
    </div>
  </section>
</template>

<style scoped>
@keyframes slide {
  from {
    transform: translate3d(0, 0, 0);
  }
  to {
    transform: translate3d(-1100px, 0, 0);
  }
}

.slider:hover .slide-track {
  animation-play-state: paused;
}

.slide-track {
  animation: 15s slide infinite alternate linear;
}
</style>
