<script>
  import Subheader from "../../lib/Subheader.svelte";

  let pageTitle = 'Our clients'
</script>

<svelte:head><title>{pageTitle} • Mtt</title></svelte:head>
<div class="main">
  <Subheader pageTitle={pageTitle}/>
  <h1>Work in progress</h1>
</div>

<style>
  .main {
    display: flex;
    flex-direction: column;
    width: 100%;
  }
</style>