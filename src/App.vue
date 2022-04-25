<script setup lang="ts">
import { ref, watch } from '@vue/composition-api';

const foo = ref('');
watch([foo] as const, ([foo]) => {
  console.log(foo.length);
})
</script>

<template>
  <div id="app" />
</template>
