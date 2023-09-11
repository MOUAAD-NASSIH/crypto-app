<script setup>
import TopRightArrow from "../icons/TopRightArrow.vue";

const props = defineProps({
  theme: String,
});
</script>

<template>
  <button
    :class="'border-' + props.theme"
    class="px-2 py-2 rounded-full border-[1px] md:border-2"
  >
    <TopRightArrow :color="'text-' + props.theme" />
  </button>
</template>
