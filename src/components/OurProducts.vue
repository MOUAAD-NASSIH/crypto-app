<script setup>
import TopRightArrowButton from "./Composables/TopRightArrowButton.vue";
import LeftArrow from "./icons/LeftArrow.vue";
import RightArrow from "./icons/RightArrow.vue";
import Wallet from "./icons/Wallet.vue";
</script>

<template>
  <section class="py-10">
    <div class="container px-3">
      <div class="flex items-center justify-between px-3 mb-5">
        <h1 class="text-2xl sm:text-3xl md:text-4xl lg:text-5xl font-semibold">
          Our products
        </h1>
        <div class="flex items-center gap-3 md:gap-6 lg:gap-8">
          <button
            class="p-1 md:p-2 rounded-full border-[1px] md:border-2 border-gray-700 cursor-pointer"
          >
            <LeftArrow />
          </button>
          <button
            class="p-1 md:p-2 rounded-full border-[1px] md:border-2 border-gray-700 cursor-pointer"
          >
            <RightArrow />
          </button>
        </div>
      </div>

      <div
        class="grid grid-cols-4 sm:grid-cols-10 lg:grid-cols-12 gap-4 md:gap-6"
      >
        <div
          class="col-span-4 sm:col-span-6 lg:col-span-8 text-white bg-[#1a1a24] py-6 px-3 md:py-8 lg:py-9 xl:py-10 md:px-5 lg:px-10 xl:px-16 rounded-3xl space-y-5 lg:space-y-7"
        >
          <button
            class="bg-[#fdc8e6] px-3 py-1 flex items-center gap-2 rounded-full"
          >
            <Wallet />
            <span class="text-black md:text-[17px] lg:text-lg">Wallet</span>
          </button>
          <h2
            class="text-2xl sm:text-3xl lg:text-5xl lg:leading-[3.2rem] font-semibold"
          >
            The Easiest and Most <br />
            Powerful Crypto Wallet
          </h2>
          <p
            class="max-w-[370px] sm:max-w-[420px] sm:text-[17px] lg:text-lg font-thin"
          >
            Buy Bitcoin instantly with a credit card, debit card, or by linking
            your bank.
          </p>
          <button class="flex items-center gap-3 md:gap-4">
            <TopRightArrowButton theme="pink-300" />
            <span class="text-pink-300 font-semibold md:text-[17px] lg:text-lg"
              >Start</span
            >
          </button>
        </div>
        <div class="col-span-4 flex flex-col gap-1">
          <div
            class="bg-white rounded-3xl px-3 py-3 flex items-center justify-center border-black border-[1px] md:border-2"
          >
            <h3 class="text-7xl md:text-8xl">
              10<span class="text-3xl">%</span>
            </h3>
            <p
              class="font-semibold text-center max-w-[122px] md:text-[17px] lg:text-lg"
            >
              Earn with us in rewards
            </p>
          </div>
          <div
            class="bg-[#fdc8e6] rounded-3xl px-3 py-3 flex flex-col items-center justify-center border-black border-[1px] md:border-2"
          >
            <h3 class="text-7xl md:text-8xl">
              100<span class="text-3xl">%</span>
            </h3>
            <p class="font-semibold text-center md:text-[17px] lg:text-lg">
              Your crypto in one place
            </p>
          </div>
        </div>

        <div></div>
      </div>
    </div>
  </section>
</template>
