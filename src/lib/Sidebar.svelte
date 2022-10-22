<script>
  import SideItem from "$lib/SideItem.svelte";

  let sideItems = [
    {
      title: 'Our consultants',
      link: '',
    },
    {
      title: 'Who we are',
      link: '',
    },
    {
      title: 'Our services',
      link: '',
    },
    {
      title: 'Our clients',
      link: '',
    },
    {
      title: 'Vacancies',
      link: '',
    },
    {
      title: 'HRCI Certification',
      link: '',
    },
    {
      title: 'Digital Tool in Recruitment',
      link: '',
    },
    {
      title: 'Contact us',
      link: '',
    },
  ]
</script>
<div class="sidebar">
  {#each sideItems as button}
  <SideItem title={button.title} link={button.link}/>
  {/each}
</div>

<style>
  .sidebar {
    margin: 0 20px;
  }
</style>

