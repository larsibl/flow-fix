<script lang="ts">
  export let number: number;

  let completed: boolean = false;

  function toggleCompleted() {
    completed = !completed;
  }
</script>

<button class={completed ? 'completed' : ''} on:click={toggleCompleted}>
  {completed ? number : ''}
</button>

<style lang="postcss">
  @reference 'tailwindcss';

  button {
    @apply border-12 border-stone-600 h-36 rounded-full w-36 hover:bg-stone-800;
  }

  button.completed {
    @apply bg-stone-600 font-extrabold text-6xl;
  }
</style>
