<script setup>
import ExchangeBitcoin from '../icons/ExchangeBitcoin.vue';
import ExchangeCandle from '../icons/ExchangeCandle.vue';
</script>

<template>
  <div class="w-full border-2 border-black rounded-2xl p-2 sm:px-6 sm:py-4 md:p-2 lg:px-8 lg:py-6">
      <div class="flex justify-between py-2">
        <slot name="logo"></slot>
        <div class="flex flex-col gap-2 items-end">
          <button class="p-[2px] sm:px-2 sm:py-1 flex items-center gap-2 bg-[#eeebfe] rounded-full">
            <ExchangeBitcoin /> <span class="text-[12px] sm:text-sm uppercase text-[#6934cd]">Buy</span>
          </button>
          <button class="p-[2px] sm:px-2 sm:py-1 flex items-center gap-1 bg-[#e5faeb] rounded-full">
            <ExchangeCandle /> <span class="text-[12px] sm:text-sm uppercase text-[#17a657]">Trade</span>
          </button>
        </div>
      </div>
      <div class="py-2 font-mono">
        <p class="flex items-center gap-2 text-lg font-semibold">
          <span class="tracking-wide lg:tracking-wider">
            <slot name="curr-title"></slot>
          </span>
          <span class="uppercase text-gray-500 text-xl font-medium">
            <slot name="curr-abr"></slot>
          </span>
        </p>
        <p class="flex items-center gap-6 ">
          <span class="text-gray-600">
            <slot name="curr-val"></slot>
          </span>
          <span class="text-[#17a657]">
            <slot name="curr-perc"></slot>
          </span>
        </p>
      </div>
  </div>
</template>
