<template>
  <footer class="absolute top-0 right-0 left-0 grid grid-cols-3 px-8 py-4 text-xs">
    <div class="flex items-center gap-10">
      <span>{{ $slidev.configs.presentedBy }}</span>
      <div class="border-yukino-border flex-1 border-b opacity-30" />
    </div>
    <div class="flex items-center gap-10">
      <div class="border-yukino-border flex-1 border-b opacity-30" />
      <span>{{ $slidev.configs.title }}</span>
      <div class="border-yukino-border flex-1 border-b opacity-30" />
    </div>
    <div class="flex items-center gap-10">
      <div class="border-yukino-border flex-1 border-b opacity-30" />
      <span>{{ $slidev.nav.currentPage }}</span>
    </div>
  </footer>
</template>
