<script lang="ts">
  const navItems = [
    { title: 'Home', link: '/' },
    { title: 'Product', link: '/product' },
    { title: 'Pricing', link: '/pricing' },
    { title: 'About Us', link: '/about' },
    { title: 'Blog', link: '/blog' },
    { title: 'Contact', link: '/contact' }
  ]
</script>

<nav>
  {#each navItems as item}
    <a class="link" data-sveltekit-preload-data="hover" href={item.link}>
      {item.title}
    </a>
  {/each}
</nav>

<style>
  nav {
    display: flex;
    gap: 32px;
  }

  .link {
    font-size: 18px;
    border-bottom: 1px solid transparent;

    &:hover {
      border-bottom: 1px solid #1D2130;
    }
  }
</style>
