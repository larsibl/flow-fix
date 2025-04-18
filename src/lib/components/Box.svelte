<script lang="ts">
  let completed: boolean = false;

  function toggleCompleted() {
    completed = !completed;
  }
</script>

<button class={completed ? 'completed' : ''} on:click={toggleCompleted}>
  {completed ? '✅' : '☑️'}
</button>

<style lang="postcss">
  @reference 'tailwindcss';

  button {
    @apply bg-gray-800 h-full rounded-2xl w-full;
  }

  button.completed {
    @apply bg-green-800;
  }
</style>
