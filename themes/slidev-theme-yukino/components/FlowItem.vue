<script setup lang="ts">
interface Props {
  title: string;
  description?: string;
  icon?: string;
}

withDefaults(defineProps<Props>(), {
  description: '',
  icon: '*',
});
</script>

<style>
.yukino-flow-item {
  display: grid;
  grid-template-columns: 2rem minmax(0, 1fr);
  align-items: start;
  column-gap: 0.85rem;
  padding: 0.52rem 0.12rem;
}

.yukino-flow-icon {
  color: var(--yukino-accent);
  font-size: 0.92rem;
  font-weight: 700;
}

.yukino-flow-copy h4 {
  margin: 0.04rem 0 0.1rem;
}

.yukino-flow-copy p {
  margin: 0;
}
</style>

<template>
  <article class="yukino-flow-item">
    <div
      class="yukino-flow-icon bg-yukino-accent-soft grid h-8 w-8 place-content-center rounded"
      aria-hidden="true"
    >
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
