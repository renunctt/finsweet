<script lang="ts">
    import SecondHeading from "./ui/SecondHeading.svelte"
    import encryptionIcon from '../assets/icons/encryption.svg'
    import toolsIcon from '../assets/icons/tools.svg'
    import aiIcon from '../assets/icons/ai.svg'

    const features = [
      { icon: encryptionIcon, title: 'Advanced 256-bit encryption', desc: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor.' },
      { icon: toolsIcon, title: 'Simple collaboration tools', desc: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor.' },
      { icon: aiIcon, title: 'Customizable AI features', desc: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor.' },
    ]
</script>

<section class="section">
  <div class="container">
    <SecondHeading>Features</SecondHeading>
    <div class="features">
      {#each features as featur}
        <div class="featur">
          <img src={featur.icon} alt={featur.title} />
          <h3>{featur.title}</h3>
          <p>{featur.desc}</p>
        </div>
      {/each}
    </div>
  </div>
</section>

<style>
  .section {
    margin-top: 128px;
  }

  .container {
    width: 1280px;
    text-align: center;
    margin: 0 auto;
    padding: 0 15px;
  }

  .features {
    display: flex;
    justify-content: space-between;
    background-color: rgba(215, 152, 225, 0.15);
    border-radius: 24px;
    margin-top: 54px;
    padding: 64px;
    text-align: start;
  }

  .featur {
    width: 339px;
  }

  h3 {
    font-weight: 700;
    font-size: 36px;
    line-height: 1.2;
    margin: 24px 0 16px;
  }

</style>
