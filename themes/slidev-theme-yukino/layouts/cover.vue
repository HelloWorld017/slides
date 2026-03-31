<script setup lang="ts">
interface Props {
  presentedAt?: string;
  presentedBy?: string;
}

defineProps<Props>();
</script>

<style>
.yukino-cover-shell p {
  font-weight: 500;
}
</style>

<template>
  <div class="slidev-layout cover flex h-full flex-col">
    <div class="yukino-cover-shell flex flex-1 flex-col items-end justify-center">
      <slot />
    </div>
    <div class="yukino-cover-items flex flex-0 gap-8 text-sm">
      <div class="yukino-cover-item flex flex-col" v-if="presentedAt">
        <strong class="font-[Metropolis] font-medium uppercase">Presented At</strong>
        <span class="font-bold">{{ presentedAt }}</span>
      </div>
      <div class="yukino-cover-item flex flex-col" v-if="presentedBy">
        <strong class="font-[Metropolis] font-medium uppercase">Presented By</strong>
        <span class="font-bold">{{ presentedBy }}</span>
      </div>
    </div>
  </div>
</template>
