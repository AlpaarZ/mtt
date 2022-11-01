<script>
  import Sidebar from "$lib/Sidebar.svelte";

  let showMobileMenu = false;
</script>


<header>
  <a href="/"><img src="/Logo.png" alt="logo"></a>
  <!-- svelte-ignore a11y-click-events-have-key-events -->
  <svg class="hamburger" viewBox="0 0 100 80" width="30" height="30">
    <rect width="100" height="5" rx="5" fill="white"></rect>
    <rect y="30" width="100" height="5" rx="5" fill="white"></rect>
    <rect y="60" width="100" height="5" rx="5" fill="white"></rect>
  </svg>
</header>
<div class="main">
  <div class="sidebar">
    <Sidebar />
  </div>
  <div class="slot">
    <slot></slot>
  </div>
</div>
<div class="footer">
  <p>Copyright © 2022 Mtt </p>
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
    background: #0f0f0f; 
  }
  header img {
    width: 10rem;
    user-select: none;
  }
  .hamburger {
    display: none;
    color: #fff;
    align-items: center;
  }
  .main {
    display: flex;
    flex-direction: row;
    width: 100%;
  }
  .slot {
    flex-grow: 1;
  }
  @media screen and (max-width: 768px) {
    header {
      justify-content: space-between;
    }
    .sidebar {
      display: none;
    }
    .hamburger {
      display: flex;
    }
  }
  .footer p {
    color: white;
    text-align: center;
    font-weight: 200;
    padding: 1rem;
  }
</style>
