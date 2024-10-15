<script>
  import { Sidebar, SidebarGroup, SidebarItem, SidebarWrapper } from 'flowbite-svelte';
</script>

<Sidebar>
  <SidebarWrapper>
    <SidebarGroup>
      <!-- <SidebarBrand {site} /> -->
      <SidebarItem href="/" label="Home" />
      <SidebarItem href="/about" label="About" />
    </SidebarGroup>
  </SidebarWrapper>
</Sidebar>
