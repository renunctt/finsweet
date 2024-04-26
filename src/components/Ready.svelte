<script lang="ts">
  import BaseButton from './ui/BaseButton.svelte'
  import SecondHeading from './ui/SecondHeading.svelte'
</script>

<section class="section">
  <SecondHeading>Are you ready to grow your business with us?</SecondHeading>
  <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy.</p>
  <BaseButton>View Pricing</BaseButton>
</section>

<style>
  .section {
    width: 700px;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    margin: 128px auto 0;
    padding: 0 15px;
  }

  p {
    margin: 24px 0 32px;
  }
</style>
