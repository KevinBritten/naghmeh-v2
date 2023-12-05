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
    <nav class="flex justify-center">
      <nuxt-link
        :to="`/${pageName.toLowerCase()}`"
        v-for="pageName in pageNames"
        :key="pageName"
        class="text-xl mx-4 text-white hover:text-gray-800"
      >
        {{ pageName.toUpperCase() }}
      </nuxt-link>
    </nav>

    <!-- Language button on the right -->
    <button
      class="text-lg text-white hover:text-gray-800"
      @click="switchLanguage"
    >
      FR
    </button>
  </header>
</template>

<script>
export default {
  data() {
    return {
      pageNames: [
        "Home",
        "About",
        "Music",
        "Store",
        "Videos",
        "Photos",
        "Contact",
        "Shows",
        "Press",
      ],
    };
  },
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
