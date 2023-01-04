<script setup lang="ts">
import { ref } from 'vue';
import RecipeCard from '../components/RecipeCard.vue';

const recipes = ref(['1', '2', '3', '4', '5']);
</script>

<template>
  <q-page padding class="q-px-xl">
    <span class="text-h2">Recipes</span>
    <div class="q-pa-md row items-start">
      <RecipeCard
        v-for="recipe in recipes"
        :key="recipe"
        :id="recipe"
        title="recipe"
        class="col-3 q-pa-sm"
      />
    </div>
  </q-page>
</template>

<style lang="sass" scoped></style>
