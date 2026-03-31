<script setup lang="ts">
interface Props {
  eyebrow?: string
  title?: string
  subtitle?: string
}

withDefaults(defineProps<Props>(), {
  eyebrow: '',
  title: '',
  subtitle: '',
})
</script>

<template>
  <header class="yukino-section-lead">
    <p v-if="eyebrow" class="text-sm uppercase font-[Metropolis] font-medium">{{ eyebrow }}</p>

    <h2 v-if="title" class="mt-4 mb-2">{{ title }}</h2>
    <h2 v-else-if="$slots.title" class="mt-4 mb-2">
      <slot name="title" />
    </h2>

    <p v-if="subtitle" class="mb-8">{{ subtitle }}</p>
    <p v-else-if="$slots.default" class="mb-8">
      <slot />
    </p>
  </header>
</template>
