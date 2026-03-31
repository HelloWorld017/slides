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

<template>
  <article class="yukino-feature-item flex flex-col items-center text-center gap-2">
    <div
      class="grid h-12 w-12 text-2xl place-content-center"
      aria-hidden="true"
    >
      <slot name="icon">
        <span>{{ icon }}</span>
      </slot>
    </div>

    <div class="yukino-flow-copy">
      <h4 class="text-base">{{ title }}</h4>
      <p v-if="description" class="text-sm opacity-80">{{ description }}</p>
      <p v-else-if="$slots.default" class="text-sm opacity-80">
        <slot />
      </p>
    </div>
  </article>
</template>
