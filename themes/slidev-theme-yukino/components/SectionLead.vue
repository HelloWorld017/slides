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
    <p v-if="eyebrow" class="yukino-kicker">{{ eyebrow }}</p>

    <h2 v-if="title">{{ title }}</h2>
    <h2 v-else-if="$slots.title">
      <slot name="title" />
    </h2>

    <p v-if="subtitle" class="yukino-subtitle">{{ subtitle }}</p>
    <p v-else-if="$slots.default" class="yukino-subtitle">
      <slot />
    </p>
  </header>
</template>
