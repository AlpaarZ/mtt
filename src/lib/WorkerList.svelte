<script>
  import WorkerItem from "$lib/WorkerItem.svelte";
  
  let WorkerList = [
    {name: 'Nargiz', image: '/', link: ''},
    {name: '', image: '', link: ''},
    {name: '', image: '', link: ''},
    {name: '', image: '', link: ''},
    {name: '', image: '', link: ''},
    {name: '', image: '', link: ''},
    {name: '', image: '', link: ''},
    {name: '', image: '', link: ''},
    {name: '', image: '', link: ''},
    {name: '', image: '', link: ''},
    {name: '', image: '', link: ''},
    {name: '', image: '', link: ''},
    {name: '', image: '', link: ''},
    {name: '', image: '', link: ''},
  ]
</script>

<div class="main">
  {#each WorkerList as worker}
  <WorkerItem name={worker.name} image={worker.image}, link={worker.link}/>
  {/each}
</div>
<img src="" alt="">

<style>
  .main {
    display: grid;
    grid-template-columns: 200px 200px 200px;
    gap: 10px;
  }
</style>