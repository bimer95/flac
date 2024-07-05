<template>
  <main class="main-content">
    <section class="main-content__section">
      <h1 class="main-content__title">Welcome to Our Website</h1>
      <p class="main-content__text">
        This is where the main content of the website will go. You can add more sections, articles, images, or any other content you want to display.
      </p>
    </section>
  </main>
</template>

<script>
export default {
  name: 'MainContent',
};
</script>

<style scoped>
.main-content {
  flex-grow: 1;
  padding: 20px;
  background-color: #f8f8f8;
}

.main-content__section {
  max-width: 1200px;
  margin: 0 auto;
}

.main-content__title {
  font-size: 2em;
  margin-bottom: 20px;
}

.main-content__text {
  font-size: 1.2em;
  line-height: 1.6;
}
</style>
