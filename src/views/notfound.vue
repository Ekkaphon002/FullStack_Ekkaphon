<template>
  <div class="min-h-screen flex flex-col items-center justify-center bg-blue-50 text-center px-4 font-sans">
    <h1 class="text-6xl font-bold text-blue-700 mb-4">404</h1>
    <p class="text-lg text-blue-800 mb-6">
      The page you're looking for doesn't exist.
    </p>
    <button
      @click="goHome"
      class="px-6 py-2 bg-blue-500 text-white rounded hover:bg-blue-600 transition"
    >
      Go to Home
    </button>
  </div>
</template>

<script>
export default {
  name: 'NotFoundView',
  methods: {
    goHome() {
      this.$router.push('/');
    },
  },
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Prompt&display=swap');

.font-sans {
  font-family: 'Prompt', sans-serif;
}
</style>
