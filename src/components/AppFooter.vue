<script setup>
const socials = [
  {
    name: "Twitter",
    link: "http://x.com",
  },
  {
    name: "Instagram",
    link: "http://instagram.com",
  },
  {
    name: "Medium",
    link: "http://medium.com",
  },
];

const navigation = [
  {
    name: "Products",
    links: ["Wallet", "Exchange", "Explorer", "Learn"],
  },
  {
    name: "Resources",
    links: [
      "APIs",
      "Status",
      "Open Source",
      "Research",
      "Wallet Support",
      "Blog",
    ],
  },
  {
    name: "Company",
    links: ["About", "Careers", "Press Center", "Prime", "Ventures", "BCAM"],
  },
];
</script>

<template>
  <section class="pt-10 pb-5 px-5 bg-slate-300/10">
    <div class="flex flex-col sm:flex-row gap-8">
      <div class="sm:flex-1 space-y-4 sm:space-y-8">
        <div
          class="flex flex-col gap-3 justify-center items-center sm:items-start"
        >
          <img class="w-14" src="../assets/logo.png" alt="logo" />
          <div class="flex gap-5">
            <a
              class="text-sm font-serif"
              v-for="social in socials"
              :key="social.name"
              :href="social.link"
            >
              {{ social.name }}</a
            >
          </div>
        </div>
        <div class="hidden flex-col gap-2 sm:flex text-gray-600">
          <p class="text-[14px]">
            For further details see our Legal Disclosures. By using this
            website, you accept our Terms of Use and Privacy Policy. O Copyright
            2022. Blockchain LLC. All rights reserved.
          </p>
          <span class="text-[14px]"
            >© Copyright 2022. Blockchain LLC. All rights reserved.</span
          >
        </div>
      </div>

      <div class="sm:flex-1 space-y-4 sm:mt-10">
        <div class="flex flex-wrap gap-6 justify-around">
          <div v-for="nav in navigation" :key="nav.name">
            <h2 class="font-semibold text-lg mb-3">{{ nav.name }}</h2>
            <ul class="space-y-2">
              <li
                class="font-sans text-gray-600 text-[14px]"
                v-for="(sub, index) in nav.links"
                :key="index"
              >
                {{ sub }}
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="mt-8 flex flex-col gap-6 sm:hidden text-gray-500">
      <p class="text-[14px]">
        For further details see our Legal Disclosures. By using this website,
        you accept our Terms of Use and Privacy Policy. O Copyright 2022.
        Blockchain LLC. All rights reserved.
      </p>
      <span class="text-[14px]"
        >© Copyright 2022. Blockchain LLC. All rights reserved.</span
      >
    </div>
  </section>
</template>
