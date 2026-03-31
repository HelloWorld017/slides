<style>
  .yukino-contents > * {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center;
  }
</style>

<template>
  <div class="slidev-layout">
    <div class="yukino-contents-left-shell h-full min-h-0 flex gap-12">
      <div class="yukino-contents w-[40%] h-[calc(100%+2rem)] -ml-12 -my-4">
        <slot name="left"/>
      </div>
      <div>
        <slot />
      </div>
    </div>
  </div>
</template>
