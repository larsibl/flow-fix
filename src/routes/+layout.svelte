<script lang="ts">
  import '../app.css';

  let { children } = $props();
</script>

{@render children()}

<style lang="postcss">
  @reference "tailwindcss";

  :global(html) {
    @apply bg-stone-950 h-full;
  }

  :global(body) {
    @apply h-full;
  }
</style>
