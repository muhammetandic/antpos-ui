<script lang="ts">
  import Container from '$lib/components/base/containers/container.svelte';
  import Text from '$lib/components/base/typo/text.svelte';
  import Youtube from '$lib/images/youtube.svelte';
  import Instagram from '$lib/images/instagram.svelte';
  import Linkedin from '$lib/images/linkedin.svelte';

  let year = new Date().getFullYear();
</script>

<footer>
  <Container
    basic
    rounded
    padding="p-2 sm:p-4"
    className="flex justify-between items-center bg-secondary"
  >
    <div><Text inline size="sm">© {year} AntPos.</Text></div>
    <div class="flex">
      <a href="https://youtube.com/"> <Youtube size={20} /> </a>
      <a href="https://linkedin.com/" class="ml-3 sm:ml-6"> <Linkedin size={20} /> </a>
      <a href="https://instagram.com/" class="ml-3 sm:ml-6"> <Instagram size={20} /> </a>
    </div>
    <ul class="text-sm sm:flex sm:flex-wrap sm:items-center">
      <li><a href="about" class="mr-4 hover:underline md:mr-6">Hakkında</a></li>
      <li><a href="kvkk" class="mr-4 hover:underline md:mr-6">KVKK</a></li>
      <li><a href="contact" class="hover:underline">İletişim</a></li>
    </ul>
  </Container>
</footer>
