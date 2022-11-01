<script>
  import SideItem from "$lib/SideItem.svelte";

  let sideItems = [
    {
      title: 'Our consultants',
      link: '/',
    },
    {
      title: 'Who we are',
      link: '/who-we-are',
    },
    {
      title: 'Our services',
      link: '/our-services',
    },
    {
      title: 'Our clients',
      link: '/our-clients',
    },
    {
      title: 'Vacancies',
      link: '/vacancies',
    },
    {
      title: 'HRCI Certification',
      link: '/hrci-certification',
    },
    {
      title: 'Digital tools',
      link: '/digital-tools',
    },
    {
      title: 'Contact us',
      link: '/contact-us',
    },
  ]
</script>
<div class="sidebar">
  {#each sideItems as button}
  <SideItem title={button.title} link={button.link}/>
  {/each}
  <div class="social">
    <a href="https://www.linkedin.com/company/mtt-llc/" target="_blank" rel="noreferrer external"><img src="/linkedin-fav.png" alt=""></a>
    <a href="https://www.instagram.com/mtt.az/" target="_blank" rel="noreferrer external"><img src="/insta-fav.png" alt=""></a>
  </div>
</div>

<style>
  .sidebar {
    padding: 5.3rem 20px 0 20px;
  }
  .social {
    display: flex;
    justify-content: center;
    align-items: center;
    user-select: none;
  }
  .social img {
    width: 30px;
    margin: 0 1rem;
    cursor: pointer;

    transition: 0.08s ease-in-out;
  }
  .social img:active {
    opacity: 0.8;
  }
</style>

