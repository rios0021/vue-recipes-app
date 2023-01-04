<script setup lang="ts">
import { useRouter } from 'vue-router';

interface Props {
  id: string;
  title: string;
}

const router = useRouter();
const props = defineProps<Props>();
const onClick = () => {
  router.push(`/recipe/${props.id}`);
};
</script>
<template>
  <div>
    <q-card class="recipe-card" @click="onClick">
      <q-img src="https://cdn.quasar.dev/img/parallax2.jpg">
        <div class="text-h6 absolute-bottom text-left">{{ props.title }}</div>
      </q-img>
    </q-card>
  </div>
</template>

<style scoped>
.recipe-card {
  cursor: pointer;
}
</style>
