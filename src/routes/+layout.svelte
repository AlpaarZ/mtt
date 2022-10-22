<script>
  import Sidebar from "$lib/Sidebar.svelte";
</script>

<header>
  <img src="/Logo.png" alt="logo">
</header>
<div class="main">
  <div class="sidebar">
    <Sidebar />
  </div>
  <slot></slot>
</div>

<style>
  header {
    height: 80px;
    background-color: #191919;
  }
  header img {
    width: 10rem;
  }
  .main {
    display: flex;
    flex-direction: row;
  }
  .sidebar {
    margin-top: 20px;
  }
</style>
