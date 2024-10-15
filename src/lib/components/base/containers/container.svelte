<script lang="ts">
  export let basic: boolean | string = 'bg-gray-50 dark:bg-gray-900';
  export let rounded: boolean | string = 'rounded-lg';
  export let shadow = 'shadow';
  export let padding = 'p-0';
  export let margin = 'm-0';
  export let className = '';
</script>

<div class={`${basic} ${rounded} ${shadow} ${padding} ${margin} ${className}`}>
  <slot />
</div>
