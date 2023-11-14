<template>
  <header class="bg-transparent py-4 px-6 flex justify-between items-center">
    <!-- Logo on the left -->
    <div class="flex items-center">
      <nuxt-link
        to="/"
        class="text-blue-500 text-lg font-semibold hover:text-blue-700"
      >
        Your Logo
      </nuxt-link>
    </div>

    <!-- Navigation links centered -->
    <nav class="flex justify-center space-x-6">
      <nuxt-link to="/" class="text-gray-800 hover:text-blue-500"
        >HOME</nuxt-link
      >
      <nuxt-link to="/about" class="text-gray-800 hover:text-blue-500"
        >ABOUT</nuxt-link
      >
      <nuxt-link to="/music" class="text-gray-800 hover:text-blue-500"
        >MUSIC</nuxt-link
      >
      <nuxt-link to="/store" class="text-gray-800 hover:text-blue-500"
        >STORE</nuxt-link
      >
      <nuxt-link to="/videos" class="text-gray-800 hover:text-blue-500"
        >VIDEOS</nuxt-link
      >
      <nuxt-link to="/photos" class="text-gray-800 hover:text-blue-500"
        >PHOTOS</nuxt-link
      >
      <nuxt-link to="/contact" class="text-gray-800 hover:text-blue-500"
        >CONTACT</nuxt-link
      >
      <nuxt-link to="/shows" class="text-gray-800 hover:text-blue-500"
        >SHOWS</nuxt-link
      >
      <nuxt-link to="/press" class="text-gray-800 hover:text-blue-500"
        >PRESS</nuxt-link
      >
    </nav>

    <!-- Language button on the right -->
    <button class="text-gray-800 hover:text-blue-500" @click="switchLanguage">
      FR
    </button>
  </header>
</template>

<script>
export default {
  methods: {
    switchLanguage() {
      // Add your language switching logic here
      // For now, it's a blank function
    },
  },
};
</script>

<style scoped>
/* Add any additional styling here */
</style>
