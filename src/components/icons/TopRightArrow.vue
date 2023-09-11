<script setup>
const props = defineProps({
  color: String,
});
</script>

<template>
  <svg
    :class="props.color"
    class="w-5 lg:w-6 fill-current"
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 24 24"
  >
    <path
      fill="currentColor"
      d="M6.4 18L5 16.6L14.6 7H6V5h12v12h-2V8.4L6.4 18Z"
    ></path>
  </svg>
</template>
