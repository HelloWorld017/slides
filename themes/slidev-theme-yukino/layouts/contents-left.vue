<script setup lang="ts">
interface Props {
  ratio?: number;
}

withDefaults(defineProps<Props>(), {
  ratio: 40,
});
</script>

<style>
  .yukino-contents > img, video {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center;
  }
</style>

<template>
  <div class="slidev-layout">
    <div class="yukino-contents-left-shell h-full min-h-0 flex gap-12 items-center">
      <div class="yukino-contents h-[calc(100%+2rem)] -ml-12 -my-4" :style="{ width: `${ratio}%` }">
        <slot name="left"/>
      </div>
      <div class="min-w-0 flex-[1_1_0]">
        <slot />
      </div>
    </div>
  </div>
</template>
