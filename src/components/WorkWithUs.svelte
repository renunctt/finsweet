<script lang="ts">
  import BaseHeadingLabel from './ui/BaseHeadingLabel.svelte'
  import SecondHeading from './ui/SecondHeading.svelte'
  import arrowIcon from '../assets/icons/arrow.svg'

  const items = [1, 2, 3]
</script>

<section class="section">
  <div class="container">
    <aside class="left">
      <BaseHeadingLabel>Why should you work with us?</BaseHeadingLabel>
      <SecondHeading>Why should you work with us?</SecondHeading>
      <p class="info">
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor
        invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua invidunt ut labore.
      </p>
    </aside>
    <aside class="right">
      {#each items as i}
        <div class="item" id={i.toString()}>
          <img src={arrowIcon} alt="arrow" />
          <p class="desc">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod.
          </p>
        </div>
      {/each}
    </aside>
  </div>
</section>

<style>
  .section {
    width: 100%;
    padding: 128px 0;
    background-color: #fff;
  }

  .container {
    width: 1548px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 0 auto;
  }

  .left {
    width: 576px;
    display: flex;
    flex-direction: column;
    gap: 24px;
  }

  .right {
    height: 240px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

  .info {
    line-height: 1.5;
  }

  .item {
    display: flex;
    align-items: center;
    gap: 24px;
  }

  .desc {
    width: 500px;
    font-weight: 500;
    font-size: 20px;
    line-height: 1.5;
  }
</style>
