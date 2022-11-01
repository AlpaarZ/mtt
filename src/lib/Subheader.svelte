<script>
  export let pageTitle;
</script>

<header>
  <h1 class="title">{pageTitle}</h1>
  {#if pageTitle == "Our consultants"}
  <input type="text" class="searchbar" placeholder="Search for consultants...">
  {/if}
</header>

<style>
  header {
    display: flex;
    align-items: center;
    justify-content: flex-start;
    width: 100%;
    padding: 2rem 0 1rem 0;
  }
  .title {
    font-size: 36px;
    font-weight: 200;
  }
  .searchbar {
    border: none;
    border-radius: 10px;
    background-color: #373737;
    color: white;
    font-weight: 100;
    font-size: 1.5rem;
    padding: 5px 2rem 5px .5rem;
    
    box-shadow: 0 0 10px 10px rgba(0, 0, 0, 0.1);
  }
  @media (max-width: 768px) {
    header {
      justify-content: center;
      flex-direction: column;
      text-align: center;
    }

  }
</style>