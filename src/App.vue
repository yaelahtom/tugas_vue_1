<script setup>
  import Counter from './components/Counter.vue'
  import BoxColorChanger from './components/BoxColorChanger.vue';
  import ImageCarousel from './components/ImageCarousel.vue';
</script>

<template>
  <div>
    <div class="animated-bg"></div> <!-- Div for animated background -->
    <div class="content">
      <h1>Tugas Vue</h1>
      <Counter />
      <BoxColorChanger/>
      <ImageCarousel/>
    </div>
  </div>
</template>

<style scoped>
  /* Ensure the content is displayed above the background */
  .content {
    position: relative;
    z-index: 1; /* Bring the content above the background */
    text-align: center; /* Center the content */
  }

  h1 {
    color: #42b983;
  }
</style>
