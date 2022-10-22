<script>
  import WorkerList from "$lib/WorkerList.svelte";
</script>

<div class="main">
  <header>
    <h1>Our conultants</h1>
    <input type="text" class="searchbar" placeholder="Search for consultants...">
  </header>
  
  <WorkerList />
</div>
<style>
  .main {
    display: flex;
    flex-direction: column;
    width: 100%;
  }
  header {
    display: inherit;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    margin: 20px 20px 20px 0;
  }
  header h1 {
    font-size: 36px;
    font-weight: 200;
  }
  .searchbar {
    border: none;
    border-radius: 10px;
    background-color: #373737;
    color: white;
    font-weight: 200;
    padding: 5px;
    width: 33%;
  }
</style>