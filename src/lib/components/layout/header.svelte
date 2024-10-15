<script lang="ts">
  import Container from '../base/containers/container.svelte';

  export let subtitle: string | null = null;

  let logo = {
    src: 'images/logo-no-background.png',
    alt: 'AntPos Dükkanım',
    width: '150'
  };
</script>

<Container
  basic
  rounded
  padding="p-2 sm:p-4"
  className="flex justify-between items-center bg-secondary"
>
  <div>
    <img src={logo.src} alt={logo.alt} width={logo.width} />
    {#if subtitle}
      <h2 class="text-left text-gray-700">{subtitle}</h2>
    {/if}
  </div>
</Container>
