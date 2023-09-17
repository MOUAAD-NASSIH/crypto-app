<script setup>
import CandleCharts from "./icons/CandleChart.vue";
import CustomButton from "./Composables/Button.vue";
import CurrencyInfo from "./Composables/CurrencyInfo.vue";
import ButtonIconApple from "./icons/ButtonIconApple.vue";
import ButtonIconGoogle from "./icons/ButtonIconGoogle.vue";
import LogoBitcoin from "./icons/LogoBitcoin.vue";
import LogoEthereum from "./icons/LogoEthereum.vue";
</script>

<template>
  <section class="py-10">
    <div class="container max-sm:px-2 md:max-lg:px-5 lg:max-xl:px-5">
      <h1
        class="flex flex-col items-center text-4xl font-semibold sm:text-5xl md:text-[2.30rem] lg:text-6xl"
      >
        <span class="inline-block"
          >Best way to buy
          <img
            src="../assets/currency-exchange.png"
            class="w-14 sm:w-16 md:w-18 lg:w-20 xl:w-24 inline-block"
        /></span>
        <span class="ml-10 sm:ml-16 lg:ml-20 xl:ml-36 inline-block">
          trade<CandleCharts class="mr-2" />crypto</span
        >
      </h1>
      <div
        class="mt-8 flex flex-col items-center md:flex-row md:justify-around lg:justify-center gap-4 lg:gap-20"
      >
        <img
          class="w-64 lg:w-72"
          src="../assets/hand-holding-phone.png"
          alt="image"
        />

        <div class="flex flex-col gap-4 sm:w-[500px] md:w-fit">
          <div
            class="flex flex-col items-center md:items-start gap-2 md:gap-3 lg:gap-4 text-center md:text-left mb-1 sm:mb-3"
          >
            <p
              class="text-gray-600 sm:text-lg md:text-base lg:text-lg max-w-[306px] sm:max-w-[326px] md:max-w-[326px] lg:max-w-[367px] xl:max-w-[340px]"
            >
              The world's fastest crypto-matching engine built by traders for
              traders.
            </p>
            <p
              class="text-gray-600 sm:text-lg md:text-base lg:text-lg max-w-[306px] sm:max-w-[326px] md:max-w-[326px] lg:max-w-[367px] xl:max-w-[340px]"
            >
              Increased purchasing power means up to 5 times more profit.
            </p>
          </div>

          <div class="flex items-center justify-center md:justify-start gap-4">
            <CustomButton>
              <div class="flex justify-center items-center gap-2">
                <ButtonIconApple />
                <div class="flex flex-col text-sm">
                  <span class="font-thin">get app on the</span>
                  <span class="text-xl">App Store</span>
                </div>
              </div>
            </CustomButton>
            <CustomButton>
              <div class="flex justify-center items-center gap-2">
                <ButtonIconGoogle />
                <div class="flex flex-col text-sm">
                  <span class="font-thin">get app on the</span>
                  <span class="text-xl">Google Play</span>
                </div>
              </div>
            </CustomButton>
          </div>
          <div class="flex flex-row items-center md:items-start gap-2 lg:gap-6 mt-3">
            <CurrencyInfo>
              <template #logo>
                <LogoBitcoin />
              </template>
              <template #curr-title> Bitcoin </template>
              <template #curr-abr> Btc </template>
              <template #curr-val> $19.624.48 </template>
              <template #curr-perc> +2.23% </template>
            </CurrencyInfo>
            <CurrencyInfo>
              <template #logo>
                <LogoEthereum />
              </template>
              <template #curr-title> Ethereum </template>
              <template #curr-abr> Eth </template>
              <template #curr-val> $19.624.48 </template>
              <template #curr-perc> +2.23% </template>
            </CurrencyInfo>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
