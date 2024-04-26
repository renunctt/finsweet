<script lang="ts">
  import BaseHeadingLabel from './ui/BaseHeadingLabel.svelte'
  import SecondHeading from './ui/SecondHeading.svelte'

  import securityIcon from '../assets/icons/security.svg'
  import performanceIcon from '../assets/icons/performance.svg'
  import supportIcon from '../assets/icons/support.svg'

  const features = [
    {
      title: 'High security to protect from piracy',
      descr: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy.',
      icon: securityIcon
    },
    {
      title: 'Premium quality performance',
      descr: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy.',
      icon: performanceIcon
    },
    {
      title: 'Full time customer support - 24/7',
      descr: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy.',
      icon: supportIcon
    }
  ]
</script>

<section class="section">
  <div class="top">
    <BaseHeadingLabel>High-quality</BaseHeadingLabel>
    <SecondHeading>We have the Best Solution for your Business</SecondHeading>
  </div>

  <div class="features">
    {#each features as feature}
      <div class="feature">
        <img class="icon" src={feature.icon} alt="icon" />
        <h4 class="title">{feature.title}</h4>
        <p class="descr">{feature.descr}</p>
      </div>
    {/each}
  </div>
</section>

<style>
  .section {
    display: flex;
    align-items: center;
    flex-direction: column;
    margin-top: 128px;
  }

  .top {
    width: 576px;
    display: flex;
    flex-direction: column;
    text-align: center;
    gap: 24px;
    margin-bottom: 48px;
  }

  .features {
    width: 1400px;
    display: flex;
    justify-content: space-between;
    padding: 64px;
    border-radius: 24px;
    background-color: #e0e4fc;
  }

  .feature {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    width: 362px;
    height: 216px;
  }

  .icon {
    width: 48px;
    height: 48px;
  }

  .title {
    font-weight: 700;
    font-size: 32px;
    line-height: 1.2;
  }

  .descr {
    line-height: 1.5;
    opacity: 0.87;
  }
</style>
