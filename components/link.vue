<template>
  <a
    :href="url"
    data-aos="fade-up"
    :data-aos-delay="delay"
    class="flex items-center justify-center w-5/6 max-w-sm h-14 cursor-pointer p-3 m-3 mx-auto rounded-md ring-[1px] ring-green-600 backdrop-filter backdrop-blur-2xl bg-green-300 hover:bg-green-400 shadow-xl"
  >
    <Icon :name="icon" class="text-2xl text-black" />
    <h2 class="ml-2">{{ name }}</h2>
  </a>
</template>

<script setup lang="ts">
defineProps({
  url: String,
  icon: String,
  name: String,
  delay: Number,
});
</script>
