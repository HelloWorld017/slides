<template>
  <div class="slidev-layout cover yukino-cover">
    <div class="yukino-cover-main my-auto w-full">
      <slot />
    </div>
    <aside class="yukino-cover-rail" aria-hidden="true">
      <article class="yukino-rail-card">
        <p>Science Labs Essentials</p>
        <span>clarity + structure</span>
      </article>
      <article class="yukino-rail-card">
        <p>Business Strategy</p>
        <span>insight + momentum</span>
      </article>
      <article class="yukino-rail-card">
        <p>Urban Flow</p>
        <span>bold + expressive</span>
      </article>
    </aside>
  </div>
</template>
