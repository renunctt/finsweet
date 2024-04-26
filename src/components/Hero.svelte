<script lang="ts">
  import BaseHeading from './ui/BaseHeading.svelte'
  import SendForm from './ui/SendForm.svelte'
</script>

<main class="main">
  <aside class="aside">
    <BaseHeading>The Best Software to Grow your Sales and Services</BaseHeading>

    <p>
      Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor
      invidunt ut labore et dolore magna aliquyam erat.
    </p>

    <SendForm />

    <div class="gradient"></div>
  </aside>

  <div class="dashboard">
    <enhanced:img src="../assets/hero-dashboard.png" alt="dashboeard" />
  </div>
</main>

<style>
  .main,
  .aside {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .aside {
    max-width: 768px;
    text-align: center;
    margin: 96px auto 64px;
  }

  p {
    font-size: 18px;
    line-height: 1.5;
    opacity: 0.2;
  }

  .gradient {
    position: absolute;
    width: 600px;
    height: 600px;
    margin-top: 250px;
    background: radial-gradient(circle, #aed3ff 50%, #d798e1 18%, #c9d4ef 57%, #cacffa 66%);
    border-radius: 50%;
    filter: blur(300px);
    opacity: 0.5;
    z-index: -10;
  }
</style>
