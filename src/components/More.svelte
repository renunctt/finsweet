<script lang="ts">
  import BaseButton from './ui/BaseButton.svelte'
  import SecondHeading from './ui/SecondHeading.svelte'
  import moreImg from '../assets/more-img.png'
</script>

<section class="section">
  <div class="gradient">
  </div>
  <div class="container">
    <aside class="main">
      <SecondHeading>More impressions, more conversions</SecondHeading>
      <p class="desc">
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor
        invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua invidunt ut labore.
      </p>
      <BaseButton>Get Free trial</BaseButton>
    </aside>

    <aside>
      <img src={moreImg} alt="bg" />
    </aside>
  </div>
</section>

<style>
  .section {
    width: 100%;
    height: 563px;
  }

  .gradient {
    position: absolute;
    width: 100%;
    height: 563px;
    background: linear-gradient(90deg, #9bffa5 1%, #aed3ff 30%, #c9d4ef 57%, #cacffa 66%);
    filter: blur(400px);
    opacity: 0.5;
    z-index: -10;
  }

  .container {
    width: 1240px;
    height: 563px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 0 auto;
    padding: 0 15px;
  }

  .main {
    width: 576px;
  }

  .desc {
    margin: 24px 0 32px;
  }
</style>
