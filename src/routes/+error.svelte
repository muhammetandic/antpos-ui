<script lang="ts">
  import { Button } from 'flowbite-svelte';
  export let image = {
    src: 'images/404.svg',
    alt: 'astronaut'
  };
  export let mainClass = 'bg-gray-50 dark:bg-gray-900';
  export let mainDivClass =
    'flex flex-col items-center justify-center px-6 pt-8 mx-auto md:h-screen pt:mt-0 dark:bg-gray-900';
  export let h1Class =
    'mb-3 text-2xl font-bold leading-tight text-gray-900 sm:text-4xl lg:text-5xl dark:text-white';
  export let imgDiv = 'block md:max-w-lg';
  export let div2Class = 'text-center xl:max-w-4xl';
</script>

<div class={mainClass}>
  <div class={mainDivClass}>
    <div class={imgDiv}><img src={image.src} alt={image.alt} /></div>
    <div class={div2Class}>
      <h1 class={h1Class}>Page Not Found</h1>
      <Button href="/">Go Home</Button>
    </div>
  </div>
</div>
