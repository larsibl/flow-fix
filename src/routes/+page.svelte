<script lang="ts">
  import { Grid, Session } from '$lib/components';

  let sessionCount: number = $state(8);
</script>

<main>
  <Grid>
    {#each { length: sessionCount }, i}
      <div>
        <Session number={i + 1} />
      </div>
    {/each}
  </Grid>
</main>

<style lang="postcss">
  @reference 'tailwindcss';

  main {
    @apply flex flex-col h-full p-2 w-full;
  }

  div {
    @apply flex items-center justify-center;
  }
</style>
