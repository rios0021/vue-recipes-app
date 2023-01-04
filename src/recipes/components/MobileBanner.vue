<template>
  <q-card class="recipe-banner">
    <q-img src="https://cdn.quasar.dev/img/chicken-salad.jpg" />

    <q-card-section>
      <div class="row no-wrap items-center">
        <div class="col text-h6 ellipsis">Cafe Basilico</div>
      </div>

      <q-rating v-model="stars" :max="5" size="32px" />
    </q-card-section>
  </q-card>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const stars = ref(3);
</script>

<style scoped>
.recipe-banner {
  width: 100%;
}
</style>
