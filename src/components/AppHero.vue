<script setup>
import { ref } from "vue";
import Hamburger from "./icons/Hamburger.vue";
import Close from "./icons/Close.vue";
import TopRightArrowButton from "./Composables/TopRightArrowButton.vue";

const mobileNav = ref(false);
</script>

<template>
  <header class="h-[900px] sm:h-[770px] md:h-[700px] lg:h-[780px] xl:h-screen">
    <navk
      class="relative container flex items-center justify-between max-sm:px-2 md:max-xl:px-4 py-2 md:py-4"
    >
      <div class="flex items-center gap-10 lg:gap-16">
        <a href="#" class="flex-center">
          <img class="w-14 md:w-16" src="../assets/logo.png" alt="logo.png" />
        </a>
        <div class="hidden md:flex items-center gap-5 lg:gap-7 xl:gap-10">
          <a class="lg:text-lg" href="#wallet">Wallet</a>
          <a class="lg:text-lg" href="#exchange">Exchange</a>
          <a class="lg:text-lg" href="#explorer">Explorer</a>
          <a class="lg:text-lg" href="#institutional">Institutional</a>
        </div>
      </div>
      <div class="flex items-center gap-3 md:gap-5 lg:gap-7">
        <a href="#">Log in</a>
        <a
          href="#"
          class="bg-white px-3 py-1 md:px-5 md:py-2 lg:px-6 border-[1.5px] md:border-2 border-black rounded-full"
        >
          Sign up
        </a>
        <Hamburger
          @click="mobileNav = !mobileNav"
          class="block md:hidden cursor-pointer"
        />
        <Transition name="mobile-nav">
          <div
            v-show="mobileNav"
            class="bg-gray-400 fixed top-0 left-0 h-screen w-full z-50"
          >
            <div class="relative flex flex-col h-screen w-full">
              <Close
                class="absolute right-3 top-3 cursor-pointer"
                @click="mobileNav = false"
              />
              <a
                @click="mobileNav = false"
                href="#wallet"
                class="border-b border-white h-1/4 flex justify-center items-center text-white hover:text-gray-300 hover:bg-gray-600 font-bold text-4xl transition-colors duration-300"
                >Wallet</a
              >
              <a
                @click="mobileNav = false"
                href="#exchange"
                class="border-b border-white h-1/4 flex justify-center items-center text-white hover:text-gray-300 hover:bg-gray-600 font-bold text-4xl transition-colors duration-300"
                >Exchange</a
              >
              <a
                @click="mobileNav = false"
                href="#explorer"
                class="border-b border-white h-1/4 flex justify-center items-center text-white hover:text-gray-300 hover:bg-gray-600 font-bold text-4xl transition-colors duration-300"
                >Explorer</a
              >
              <a
                @click="mobileNav = false"
                href="#institutional"
                class="border-b border-white h-1/4 flex justify-center items-center text-white hover:text-gray-300 hover:bg-gray-600 font-bold text-4xl transition-colors duration-300"
                >Institutional</a
              >
            </div>
          </div>
        </Transition>
      </div>
    </navk>

    <div
      class="container grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-6 py-10 max-sm:px-2 md:max-lg:px-5 lg:max-xl:px-5"
    >
      <h1
        class="text-3xl sm:text-5xl md:text-4xl lg:text-5xl xl:text-7xl space-y-2 md:space-y-6 font-semibold md:font-bold lg:col-span-2 xl:col-span-4 flex flex-col items-center justify-center -ml-5 sm:-ml-8 lg:-ml-10 xl:-ml-18"
      >
        <span>The best lightning</span>
        <span class="ml-10 sm:ml-16 lg:ml-20 xl:ml-36 inline-block">
          crypto<img
            src="../assets/currency-exchange.png"
            class="w-14 sm:w-16 md:w-14 lg:w-20 xl:w-24 inline-block"
          />trading
        </span>
      </h1>
      <div class="flex-center flex-col gap-4 mt-8 xl:col-span-2 xl:items-start">
        <p
          class="text-center text-gray-600 lg:text-lg max-w-[372px] md:max-w-[306px] lg:max-w-[367px] xl:max-w-[340px]"
        >
          Trusted by millions since 2011 with over $1 Trillion in crypto
          transactions.
        </p>
        <div
          class="flex items-center justify-center gap-4 lg:w-[21rem] xl:w-[22rem]"
        >
          <button
            class="bg-black text-white lg:text-lg py-2 px-5 space-x-2 rounded-full"
          >
            Get Started
          </button>
          <button class="flex items-center gap-2 lg:text-lg">
            <TopRightArrowButton /> Explore
          </button>
        </div>
      </div>
    </div>

    <div class="container relative py-10">
      <div
        class="absolute transform scale-90 top-0 left-0 w-full h-full border-2 border-gray-200 bg-white rounded-3xl"
      ></div>
      <div
        class="absolute transform scale-95 top-6 left-0 w-full h-full border-2 border-gray-300 bg-white rounded-3xl"
      ></div>
      <div
        class="absolute top-12 left-0 w-full h-fit border-2 border-black bg-white rounded-3xl p-4 sm:p-6 md:p-7 lg:p-8 xl:p-10 flex flex-col-reverse items-center gap-8 sm:flex-row sm:justify-between lg:justify-around"
      >
        <div
          class="flex flex-col items-center sm:items-start gap-2 sm:gap-4 md:gap-6 lg:gap-8"
        >
          <h3
            class="text-2xl sm:leading-10 lg:leading-[4rem] sm:text-3xl lg:text-5xl font-semibold text-center sm:text-left"
          >
            The Most Trusted<br />Crypto Platform
          </h3>
          <p
            class="text-center sm:text-left md:text-lg lg:text-xl text-gray-600 font-thin"
          >
            Blockchain is the easiest place to buy and sell cryptocurrency.
            <br />
            Sign up and get started today.
          </p>
          <button class="flex items-center gap-4">
            <TopRightArrowButton />
            <span class="font-semibold text-lg lg:text-xl"
              >Get started now</span
            >
          </button>
        </div>
        <div class="xl:w-[482px]">
          <img
            class="w-48 sm:w-56 md:w-72 lg:w-80 xl:w-96"
            src="../assets/coins.png"
            alt=""
          />
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped>
.mobile-nav-enter-active,
.mobile-nav-leave-active {
  transition: 500ms ease-in-out all;
}
.mobile-nav-enter-from,
.mobile-nav-leave-to {
  transform: translateY(-800px);
}
.mobile-nav-enter-to {
  transform: translateY(0);
}
</style>
