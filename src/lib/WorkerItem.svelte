<script>
  export let name, image, link;
</script>

<div class="worker">
  <a href={link}><img src={image} alt={name}></a>
</div>

<style>
  .worker {
    display: inline-block;
    user-select: none;
    transition: 0.08s ease-in-out;
    resize: both;
  }
  .worker:hover {
    opacity: 0.8;
  }
  img {
    border-radius: 10px;
    box-shadow: 0 0 10px 5px rgba(0, 0, 0, 0.1);
  }
</style>

