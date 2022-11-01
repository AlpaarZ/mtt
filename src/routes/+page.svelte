<script>
  import WorkerList from "$lib/WorkerList.svelte";
  import Subheader from "../lib/Subheader.svelte";

  let pageTitle = 'Our consultants'
</script>
<svelte:head><title>{pageTitle} • Mtt</title></svelte:head>
<div class="main">
  <Subheader pageTitle={pageTitle}/>
  <WorkerList />
</div>
<style>
  .main {
    display: flex;
    flex-direction: column;
    flex-wrap: nowrap;
  }
</style>