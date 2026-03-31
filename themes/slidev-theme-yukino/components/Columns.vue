<script setup lang="ts">
interface Props {
  count?: number;
}

withDefaults(defineProps<Props>(), {
  count: 2,
});
</script>

<template>
  <div class="grid gap-12 items-start" :style="{ 'grid-template-columns': `repeat(${count}, 1fr)` }">
    <slot />
  </div>
</template>
