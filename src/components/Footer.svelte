<script lang="ts">
  import logoWhite from '../assets/logo-white.svg'
  import FacebookIcon from '../assets/icons/Facebook.png'
  import TwitterIcon from '../assets/icons/Twitter.png'
  import InstagramIcon from '../assets/icons/Instagram.png'
  import LinkedInIcon from '../assets/icons/LinkedIn.png'

  const items = [
    {
      title: 'Company',
      links: [
        { title: 'About Us', link: '/about' },
        { title: 'Why Choose us', link: '/#choose-use' },
        { title: 'Pricing', link: '/pricing' },
        { title: 'Testimonial', link: '/#testimonial' }
      ]
    },
    {
      title: 'Resources',
      links: [
        { title: 'Privacy Policy', link: '/privacy-policy' },
        { title: 'Terms and Condition', link: '/terms-and-condition' },
        { title: 'Blog', link: '/blog' },
        { title: 'Contact Us', link: '/contact' }
      ]
    },
    {
      title: 'Product',
      links: [
        { title: 'Marketing insights', link: '/pricing#marketing-insights' },
        { title: 'Time tracker', link: '/pricing#time-tracker' },
        { title: 'Lead generate', link: '/pricing#lead-generate' },
        { title: 'Remote teams', link: '/pricing#remote-teams' }
      ]
    }
  ]

  const icons = [
    { icon: FacebookIcon, alt: 'Facebook' },
    { icon: TwitterIcon, alt: 'Twitter' },
    { icon: InstagramIcon, alt: 'Instagram' },
    { icon: LinkedInIcon, alt: 'LinkedIn' }
  ]
</script>

<footer class="footer">
  <div class="gradient"></div>
  <div class="container">
    <div class="links">
      {#each items as item}
        <div class="item">
          <p class="title">{item.title}</p>
          {#each item.links as link}
            <a class="link" href={link.link}>{link.title}</a>
          {/each}
        </div>
      {/each}

      <div class="subscribe">
        <img src={logoWhite} width={130} alt="Logo" />
        <p class="sub-title">Subscribe to our Newsletter</p>
        <div class="form">
          <input type="email" placeholder="Enter your Email" />
          <button class="button"> Subscribe </button>
        </div>
      </div>
    </div>

    <div class="copy">
      <span class="line"></span>
      <div class="copy-info">
      <p class="copy-title">© Copyright Finsweet 2024</p>
      <div class="copy-icons">
      {#each icons as i}
        <img class="copy-icon" src={i.icon} alt={i.alt} />
      {/each}
      </div>
      </div>
      <span class="line"></span>
    </div>
  </div>
</footer>

<style>
  .line {
    width: 100%;
    height: 1px;
    background-color: #888888;
  }

  .copy-icon {
    cursor: pointer;
  }

  .copy {
    margin: 50px 0 64px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 32px;
  }

  .copy-info {
    display: flex;
    align-items: center;
    min-width: 329px;
    gap: 32px;
  }

  .copy-icons {
    display: flex;
    align-items: center;
    gap: 24px;
  }

  .copy-title {
    font-size: 12px;
    color: #fff;
    opacity: 0.6;
  }

  .subscribe {
    display: flex;
    flex-direction: column;
  }

  .sub-title {
    font-weight: 600;
    font-size: 18px;
    color: #fff;
    margin: 36px 0 16px;
  }

  .form {
    display: flex;
    width: 410px;
    height: 56px;
    border-radius: 8px;
    background-color: #2b2e3c;
  }

  input {
    width: 100%;
    background-color: #2b2e3c;
    border-radius: 8px;
    color: rgba(255, 255, 255, 0.6);
    font-size: 16px;
    padding-left: 22px;
  }

  .button {
    padding: 0 40px;
    font-weight: 500;
    border-radius: 8px;
    color: #1d2130;
  }

  .footer {
    width: 100%;
    background-color: #1d2130;
    margin-top: 128px;
  }

  .gradient {
    position: absolute;
    width: 100%;
    height: 300px;
    border-radius: 50%;
    transform: translateY(-150px);
    background: linear-gradient(90deg, #9bffa5 1%, #aed3ff 30%, #c9d4ef 57%, #cacffa 66%);
    filter: blur(100px);
    z-index: -10;
  }

  .container {
    width: 1280px;
    display: flex;
    flex-direction: column;
    margin: 0 auto;
    padding: 64px 15px 0;
  }

  .links {
    display: flex;
    gap: 58px;
  }

  .item {
    width: 230px;
    display: flex;
    flex-direction: column;
    gap: 8px;
  }

  .title {
    font-weight: 600;
    font-size: 18px;
    color: #fff;
  }

  .link {
    font-size: 16px;
    color: #fff;
    opacity: 0.6;
  }
</style>
