<script setup lang="ts">
import DesktopBanner from '../components/DesktopBanner.vue';
import MobileBanner from '../components/MobileBanner.vue';
import RecipeContent from '../components/RecipeContent.vue';
</script>

<template>
  <q-page padding class="q-px-xl">
    <MobileBanner v-if="$q.platform.is.mobile" />
    <DesktopBanner v-else />
    <RecipeContent />
  </q-page>
</template>

<style scoped></style>
