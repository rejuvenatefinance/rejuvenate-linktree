<template>
  <div
    class="flex flex-col items-center justify-center min-h-screen min-w-screen bg-gray-900 overflow-hidden pb-32"
  >
    <div
      class="h-16 md:h-24 lg:h-32 my-4"
      data-aos="fade-down"
      data-aos-delay="300"
    >
      <img src="/img/logo.png" class="h-16 md:h-24 lg:h-32" />
    </div>
    <Link
      v-for="(link, index) in links"
      :url="link.url"
      :name="link.name"
      :icon="link.icon"
      :delay="index * 100"
    />
  </div>
</template>

<style>
html,
body {
  margin: 0;
  padding: 0;
}
</style>

<script setup lang="ts">
const links = [
  {
    url: "https://rejuvenatefinance.com",
    icon: "mdi:web",
    name: "Website",
  },
  {
    url: "https://discord.com/invite/Cf2VUn4e2R",
    icon: "mdi:discord",
    name: "Discord",
  },
  {
    url: "https://t.me/+LxJTReW_wDRmMmYx",
    icon: "mdi:telegram",
    name: "Telegram",
  },
  {
    url: "https://twitter.com/rejuvenaterjv",
    icon: "mdi:twitter",
    name: "Twitter",
  },
  {
    url: "https://app.rejuvenatefinance.com",
    icon: "mdi:open-in-app",
    name: "DApp",
  },
  {
    url: "https://github.com/rejuvenatefinance",
    icon: "mdi:github",
    name: "GitHub",
  },
];
</script>
