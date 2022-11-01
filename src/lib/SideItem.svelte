<script>
export let title, link;

function openMenu() {
    isOpen = !isOpen
  }
</script>

<a on:click={openMenu} href="{link}"><div>{title}</div></a>

<style>
  div {
    background-color: var(--grey);
    padding: 20px;
    border-radius: 10px;
    font-weight: 200;
    margin-bottom: 20px;
    font-size: 1.5rem;
    text-align: center;
    user-select: none;
    min-width: max-content;

    transition: 0.08s ease-in-out;
    box-shadow: 0 0 10px 10px rgba(0, 0, 0, 0.1);
  }
  div:active {
    opacity: .8;
  }
</style>