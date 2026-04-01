<template>
  <footer
    class="bg-yukino-bg-soft text-yukino-ink-soft absolute right-4 bottom-4 flex items-center gap-4
      rounded p-2 text-sm z-1"
  >
    <lucide-circle-dashed />
    <div class="flex items-center gap-2">
      {{ $slidev.nav.currentPage }}
      <span class="border-yukino-border h-2 w-0 rotate-15 border-r" />
      {{ $slidev.nav.total }}
    </div>
  </footer>
</template>
