<script lang="ts">
  export let inline: boolean = false;
  export let size: 'xs' | 'sm' | 'md' | 'lg' | 'xl' = 'md';
  export let color: string = 'text-gray-900 dark:text-white';
</script>

{#if inline}
  <span class={`text-${size} ${color}`}><slot /></span>
{:else}
  <p class={`text-${size} ${color}`}><slot /></p>
{/if}
