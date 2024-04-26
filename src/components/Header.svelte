<script lang="ts">
  import BaseButton from './ui/BaseButton.svelte'
  import NavItems from './ui/NavItems.svelte'
</script>

<header class="header">
  <a class="logo" href="/">
    <enhanced:img src="../assets/logo.svg" alt="Logo" />
  </a>

  <div class="menu">
    <NavItems />
    <BaseButton>Free trial</BaseButton>
  </div>
</header>

<style>
  .header {
    max-width: 1410px;
    height: 70px;
    justify-content: space-between;
    margin: 0 auto;
    padding: 0 15px;
  }

  .header,
  .menu {
    display: flex;
    align-items: center;
  }

  .menu {
    gap: 32px;
  }
</style>
