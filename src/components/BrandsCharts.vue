<script setup>
import Bitcoin from "./icons/CoinBitcoin.vue";
import Ethereum from "./icons/CoinEthereum.vue";
import Xrp from "./icons/CoinXrp.vue";
import Ankr from "./icons/CoinAnkr.vue";
import Litecoin from "./icons/CoinLitecoin.vue";
import Solana from "./icons/CoinSolana.vue";
</script>

<template>
  <section class="py-10">
    <div class="flex gap-[10px] overflow-hidden select-none marqueeWrapper">
      <ul class="marquee_content">
        <li>
          <div
            class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
          >
            <Bitcoin />
            <p class="font-semibold lg:text-[18px]">Bitcoin</p>
            <button
              class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal"
            >
              +2.58%
            </button>
          </div>
        </li>
        <li>
          <div
            class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
          >
            <Ankr />
            <p class="font-semibold lg:text-[18px]">Ankr</p>
            <button
              class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal"
            >
              -2.58%
            </button>
          </div>
        </li>
        <li>
          <div
            class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
          >
            <Ethereum />
            <p class="font-semibold lg:text-[18px]">Ethereum</p>
            <button
              class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal"
            >
              +2.58%
            </button>
          </div>
        </li>
        <li>
          <div
            class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
          >
            <Litecoin />
            <p class="font-semibold lg:text-[18px]">Litecoin</p>
            <button
              class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal"
            >
              -2.58%
            </button>
          </div>
        </li>
        <li>
          <div
            class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
          >
            <Solana />
            <p class="font-semibold lg:text-[18px]">Solana</p>
            <button
              class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal"
            >
              +2.58%
            </button>
          </div>
        </li>
        <li>
          <div
            class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
          >
            <Xrp />
            <p class="font-semibold lg:text-[18px]">Xrp</p>
            <button
              class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal"
            >
              -2.58%
            </button>
          </div>
        </li>
      </ul>
      <ul class="marquee_content">
        <li>
          <div
            class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
          >
            <Bitcoin />
            <p class="font-semibold lg:text-[18px]">Bitcoin</p>
            <button
              class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal"
            >
              +2.58%
            </button>
          </div>
        </li>
        <li>
          <div
            class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
          >
            <Ankr />
            <p class="font-semibold lg:text-[18px]">Ankr</p>
            <button
              class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal"
            >
              -2.58%
            </button>
          </div>
        </li>
        <li>
          <div
            class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
          >
            <Ethereum />
            <p class="font-semibold lg:text-[18px]">Ethereum</p>
            <button
              class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal"
            >
              +2.58%
            </button>
          </div>
        </li>
        <li>
          <div
            class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
          >
            <Litecoin />
            <p class="font-semibold lg:text-[18px]">Litecoin</p>
            <button
              class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal"
            >
              -2.58%
            </button>
          </div>
        </li>
        <li>
          <div
            class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
          >
            <Solana />
            <p class="font-semibold lg:text-[18px]">Solana</p>
            <button
              class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal"
            >
              +2.58%
            </button>
          </div>
        </li>
        <li>
          <div
            class="px-6 py-3 md:px-7 md:py-4 bg-white text-black rounded-full flex items-center gap-2 md:gap-3 w-fit slide-track"
          >
            <Xrp />
            <p class="font-semibold lg:text-[18px]">Xrp</p>
            <button
              class="border-[1px] border-gray-300 rounded-full font-thin px-2 py-1 md:px-3 md:py-2 md:font-normal"
            >
              -2.58%
            </button>
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>

<style scoped>
@keyframes slide {
  0% {
    transform: translateX(0px);
  }
  100% {
    transform: translateX(calc(-100% - 10px));
  }
}

.marqueeWrapper:hover .marquee_content {
  animation-play-state: paused;
}
.marquee_content {
  animation: 15s linear 0s infinite normal forwards running slide;
  display: flex;
  flex-shrink: 0;
  gap: 10px;
  justify-content: space-around;
  min-width: 100%;
}
</style>
