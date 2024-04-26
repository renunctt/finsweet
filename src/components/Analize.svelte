<script lang="ts">
  import BaseHeadingLabel from './ui/BaseHeadingLabel.svelte'
  import SecondHeading from './ui/SecondHeading.svelte'

  import grafIcon from '../assets/icons/graf.svg'
  import personIcon from '../assets/icons/person.svg'
  import activeIcon from '../assets/icons/active.svg'

  const list = [
    {
      icon: grafIcon,
      title: 'Sales Tracking',
      desc: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr.'
    },
    {
      icon: personIcon,
      title: 'Project Management',
      desc: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr.'
    },
    {
      icon: activeIcon,
      title: 'Activity Report',
      desc: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr.'
    }
  ]
</script>

<section class="section">
  <div class="container">
    <aside class="content">
      <div class="label">
        <BaseHeadingLabel>Discover More</BaseHeadingLabel>
      </div>
      <SecondHeading>Analyze your sales and marketing leads</SecondHeading>
      <p class="desc">
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor
        invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua invidunt ut labore.
      </p>
    </aside>
    <aside class="list">
      {#each list as item}
        <div class="item">
          <img src={item.icon} alt={item.title} />
          <div class="info">
            <h4>{item.title}</h4>
            <p>{item.desc}</p>
          </div>
        </div>
      {/each}
    </aside>
  </div>
</section>

<style>
  .section {
    width: 100%;
    height: 296px;
    margin-top: 128px;
  }

  .container {
    width: 1270px;
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 0 auto;
    padding: 0 15px;
  }

  .content {
    width: 576px;
    height: 100%;
  }

  .label {
    margin-bottom: 24px;
  }

  .desc {
    margin-top: 32px;
  }

  .list {
    display: flex;
    flex-direction: column;
    gap: 40px;
  }

  .item {
    display: flex;
    align-items: center;
    gap: 32px;
  }

  h4 {
    font-weight: 700;
    font-size: 24px;
    line-height: 1.4;
  }
</style>
