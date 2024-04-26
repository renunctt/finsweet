<script>
  import Analize from '../components/Analize.svelte'
  import Comments from '../components/Comments.svelte'
  import Features from '../components/Features.svelte'
  import Hero from '../components/Hero.svelte'
  import HighQuality from '../components/HighQuality.svelte'
  import Logos from '../components/Logos.svelte'
  import More from '../components/More.svelte'
  import WorkWithUs from '../components/WorkWithUs.svelte'
</script>

<svelte:head>
  <title>Home - Finsweet</title>
</svelte:head>
<div>
  <Hero />
  <HighQuality />
  <WorkWithUs />
  <More />
  <Logos />
  <Analize />
  <Features />
  <Comments />
</div>
