<script lang="ts">
  import SecondHeading from './ui/SecondHeading.svelte'
  import clientIcon_1 from '../assets/clients/client-1.png'
  import clientIcon_2 from '../assets/clients/client-2.png'
  import clientIcon_3 from '../assets/clients/client-3.png'

  const comments = [
    {
      avatar: clientIcon_1,
      name: 'Ron Wood',
      post: 'CEO',
      desc: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.'
    },
    {
      avatar: clientIcon_2,
      name: 'Mark Mason',
      post: 'Marketing Manager',
      desc: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.'
    },
    {
      avatar: clientIcon_3,
      name: 'Sam Preston',
      post: 'CTO',
      desc: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.'
    }
  ]
</script>

<section class="section">
    <div class="heading">
      <SecondHeading>The stunning results our customers have experienced</SecondHeading>
    </div>

    <div class="comments">
      {#each comments as comment}
        <div class="comment">
          <p class="desc">{comment.desc}</p>
          <img src={comment.avatar} alt="avatar" />
          <p class="name">{comment.name}</p>
          <p class="post">{comment.post}</p>
        </div>
      {/each}
    </div>
</section>

<style>
  .section {
    width: 1280px;
    margin: 128px auto 0;
    padding: 0 15px;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .heading {
    text-align: center;
    width: 628px;
  }

  .comments {
    width: 100%;
    margin-top: 48px;
    display: flex;
    justify-content: space-between;
    gap: 24px;
  }

  .comment {
    border: 2px solid rgba(97, 153, 237, .26);
    border-radius: 24px;
    width: 411px;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 64px;
  }

  .desc {
    font-weight: 600;
    font-size: 18px;
    text-align: center;
  }

  img {
    margin-top: 25px;
  }

  .name {
    font-weight: 600;
    font-size: 20px;
    margin-top: 12px;
  }

  .post {
    font-size: 12px;
  }
</style>
