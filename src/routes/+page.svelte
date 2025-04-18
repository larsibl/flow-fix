<script lang="ts">
  import { Box, Grid } from '$lib/components';

  let boxCount: number = $state(8);
</script>

<main>
  <Grid>
    {#each { length: boxCount }}
      <Box />
    {/each}
  </Grid>
</main>

<style lang="postcss">
  @reference 'tailwindcss';

  main {
    @apply flex flex-col h-full p-2 w-full;
  }
</style>
