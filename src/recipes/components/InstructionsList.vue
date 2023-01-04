<script setup lang="ts">
import { ref } from 'vue';

const steps = ref([1, 2, 3, 4, 5]);
</script>

<template>
  <div class="text-h4 q-mt-xl">Instructions</div>
  <div v-for="step in steps" :key="step">
    <div r class="step-title">Step {{ step }}:</div>
    <div class="step-text">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Et culpa
      voluptates incidunt cum voluptatem suscipit officiis, officia veritatis
      similique corrupti enim ex quasi, eius, numquam atque qui ipsa vel rem.
    </div>
  </div>
</template>

<style lang="scss">
.step-title {
  text-decoration: underline;
  text-decoration-color: $secondary;
  text-decoration-thickness: 3px;
  margin-top: 15px;
  margin-bottom: 5px;
  font-size: 16px;
}
.step-text {
  font-size: 16px;
}
</style>
