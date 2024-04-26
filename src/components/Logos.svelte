<script lang="ts">
  import logo_1 from '../assets/icons/logo-1.svg'
  import logo_2 from '../assets/icons/logo-2.svg'
  import logo_3 from '../assets/icons/logo-3.svg'
  import logo_4 from '../assets/icons/logo-4.svg'
  import logo_5 from '../assets/icons/logo-5.svg'

  const logos = [logo_1, logo_2, logo_3, logo_4, logo_5]
</script>

<section class="section">
  <div class="container">
    {#each logos as logo}
      <button>
        <img src={logo} alt="logo" />
      </button>
    {/each}
  </div>
</section>

<style>
  .section {
    width: 100%;
    padding-top: 64px;
    background-color: #fff;
  }

  .container {
    width: 1280px;
    display: flex;
    justify-content: space-between;
    margin: 0 auto;
    padding: 0 15px 0;
  }
</style>
