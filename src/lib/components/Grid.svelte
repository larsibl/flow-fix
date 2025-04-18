<div>
  <slot />
</div>

<style lang="postcss">
  @reference 'tailwindcss';

  div {
    @apply gap-4 grid grid-cols-4 h-full w-full;
  }
</style>
