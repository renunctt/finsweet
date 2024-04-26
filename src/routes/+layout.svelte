<script>
  import Footer from '../components/Footer.svelte'
  import Header from '../components/Header.svelte'
  import Ready from '../components/Ready.svelte'
  import '../global.css'
</script>

<div class="wrapper">
  <Header />
  <slot />
  <Ready />
  <Footer />
</div>

<style>
  .wrapper {
    width: 100%;
    min-height: 100%;
    overflow: hidden;
  }
</style>
