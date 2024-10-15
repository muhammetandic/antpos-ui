<script>
  import '../app.css';
  import Footer from '$lib/components/layout/footer.svelte';
  import Header from '$lib/components/layout/header.svelte';
  import Sidebar from '$lib/components/layout/sidebar.svelte';
</script>

<div class="bg-primary p-2 sm:p-3">
  <Header subtitle="Benim İşletmem" />

  <Sidebar />

  <div class="container mx-auto min-h-[calc(100vh-285px)] p-4">
    <slot />
  </div>

  <Footer />
</div>
