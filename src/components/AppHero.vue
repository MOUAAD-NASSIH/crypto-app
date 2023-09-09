<script setup>
import { ref } from "vue";
import Hamburger from "./icons/Hamburger.vue";
import Close from "./icons/Close.vue";

const mobileNav = ref(false);
</script>

<template>
  <header class="h-screen">
    <nav
      class="relative container flex items-center justify-between max-sm:px-2 md:max-xl:px-4 py-2 md:py-4"
    >
      <div class="flex items-center gap-10 lg:gap-16">
        <a href="#" class="flex-center">
          <img
            class="w-14 md:w-16"
            src="../assets/logo.png"
            alt="logo.png"
          />
        </a>
        <div class="hidden md:flex items-center gap-5 lg:gap-7 xl:gap-10">
          <a href="#wallet">Wallet</a>
          <a href="#exchange">Exchange</a>
          <a href="#explorer">Explorer</a>
          <a href="#institutional">Institutional</a>
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
            class="bg-gray-400 fixed top-0 left-0 h-screen w-full"
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
    </nav>
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
