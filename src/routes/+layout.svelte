<script>
  import Sidebar from "$lib/Sidebar.svelte";
</script>


<header>
  <a href="/"><img src="/Logo.png" alt="logo"></a>
</header>
<div class="main">
  <div class="sidebar">
    <Sidebar />
  </div>
  <div class="slot">
    <slot></slot>
  </div>
</div>

<style>
  header {
    position: sticky;
    top: 0;
    z-index: 9999;
    width: auto;
    display: flex;
    justify-content: flex-start;
    align-items: center;
    padding: 0 3rem;
    background: rgba(25, 25, 25, 1);
  }
  header img {
    width: 10rem;
    user-select: none;
  }
  .main {
    display: flex;
    flex-direction: row;
  }
  @media screen and (max-width: 768px) {
    header {
      justify-content: center;
    }
    .sidebar {
      display: none;
    }
  }
</style>
