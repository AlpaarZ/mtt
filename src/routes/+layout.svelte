<script>
  import Sidebar from "$lib/Sidebar.svelte";
  import { fly } from "svelte/transition";

  export let isOpen = false;

  let showMobileMenu = false;
  function openMenu() {
    isOpen = !isOpen;
  }
  export function clickOutside(node) {
    const handleClick = (event) => {
      if (node && !node.contains(event.target) && !event.defaultPrevented) {
        node.dispatchEvent(new CustomEvent("click_outside", node));
      }
    };

    document.addEventListener("click", handleClick, true);

    return {
      destroy() {
        document.removeEventListener("click", handleClick, true);
      },
    };
  }
  function handleClickOutside(event) {
    isOpen = false;
  }
</script>

{#if isOpen == true}
  <div
    use:clickOutside
    on:click_outside={handleClickOutside}
    class="menu"
    transition:fly={{ duration: 300, x: 100, y: 0 }}
  >
    <Sidebar />
  </div>
  <div class="bg" transition:fly={{ duration: 300 }} />
{/if}
<header>
  <a href="/"><img src="/Logo.png" alt="logo" /></a>
  <!-- svelte-ignore a11y-click-events-have-key-events -->
  <svg
    on:click={openMenu}
    class="hamburger"
    viewBox="0 0 100 80"
    width="30"
    height="30"
  >
    <rect width="100" height="5" rx="5" fill="white" />
    <rect y="30" width="100" height="5" rx="5" fill="white" />
    <rect y="60" width="100" height="5" rx="5" fill="white" />
  </svg>
</header>
<div class="main">
  <div class="sidebar">
    <Sidebar />
  </div>
  <div class="slot" transition:fly={{ duration: 300, x: 100, y: 0 }}>
    <slot />
  </div>
</div>
<div class="footer">
  <p>Copyright © 2022 Mtt</p>
</div>

<style>
  :global(:root) {
    --dark: #0f0f0f;
    --grey: #373737;
  }
  header {
    position: sticky;
    top: 0;
    z-index: 9999;
    width: auto;
    display: flex;
    justify-content: flex-start;
    align-items: center;
    padding: 0 3rem;
    background: var(--dark);
  }
  header img {
    width: 10rem;
    user-select: none;
  }
  .hamburger {
    display: none;
    color: #fff;
    align-items: center;
    cursor: pointer;
  }
  .menu {
    position: fixed;
    top: 0;
    right: 0;
    bottom: 0;
    z-index: 9999;
    background-color: var(--dark);
  }
  .bg {
    position: fixed;
    width: 100vw;
    height: 100vh;
    z-index: 9998;
    background-color: rgba(0, 0, 0, 0.4);
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
