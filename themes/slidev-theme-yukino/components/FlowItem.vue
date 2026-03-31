<script setup lang="ts">
interface Props {
  title: string
  description?: string
  icon?: string
}

withDefaults(defineProps<Props>(), {
  description: '',
  icon: '*',
})
</script>

<template>
  <article class="yukino-flow-item">
    <div class="yukino-flow-icon" aria-hidden="true">
      <slot name="icon">
        <span>{{ icon }}</span>
      </slot>
    </div>

    <div class="yukino-flow-copy">
      <h4>{{ title }}</h4>
      <p v-if="description">{{ description }}</p>
      <p v-else-if="$slots.default">
        <slot />
      </p>
    </div>
  </article>
</template>
