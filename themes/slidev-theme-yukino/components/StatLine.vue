<script setup lang="ts">
interface Props {
  label: string
  value: string
  note?: string
}

withDefaults(defineProps<Props>(), {
  note: '',
})
</script>

<template>
  <div class="yukino-stat-line">
    <span class="yukino-stat-label">{{ label }}</span>
    <strong class="yukino-stat-value">{{ value }}</strong>
    <small v-if="note" class="yukino-stat-note">{{ note }}</small>
  </div>
</template>
