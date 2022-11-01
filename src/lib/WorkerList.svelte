<script>
  import WorkerItem from "$lib/WorkerItem.svelte";
  let WorkerList = [
    { name: "", image: "worker-img/Nargiz.jpg", link: "" },
    { name: "", image: "worker-img/Seymur.jpg", link: "" },
    { name: "", image: "worker-img/Didem.jpg", link: "" },
    { name: "", image: "worker-img/Vagif.jpg", link: "" },
    { name: "", image: "worker-img/Nargiz.jpg", link: "" },
    { name: "", image: "worker-img/Seymur.jpg", link: "" },
    { name: "", image: "worker-img/Didem.jpg", link: "" },
    { name: "", image: "worker-img/Vagif.jpg", link: "" },
    { name: "", image: "worker-img/Nargiz.jpg", link: "" },
    { name: "", image: "worker-img/Seymur.jpg", link: "" },
    { name: "", image: "worker-img/Didem.jpg", link: "" },
    { name: "", image: "worker-img/Vagif.jpg", link: "" },
    { name: "", image: "worker-img/Nargiz.jpg", link: "" },
    { name: "", image: "worker-img/Seymur.jpg", link: "" },
    { name: "", image: "worker-img/Didem.jpg", link: "" },
    { name: "", image: "worker-img/Vagif.jpg", link: "" },
    { name: "", image: "worker-img/Nargiz.jpg", link: "" },
    { name: "", image: "worker-img/Seymur.jpg", link: "" },
    { name: "", image: "worker-img/Didem.jpg", link: "" },
    { name: "", image: "worker-img/Vagif.jpg", link: "" },
    { name: "", image: "worker-img/Nargiz.jpg", link: "" },
    { name: "", image: "worker-img/Seymur.jpg", link: "" },
    { name: "", image: "worker-img/Didem.jpg", link: "" },
    { name: "", image: "worker-img/Vagif.jpg", link: "" },
    { name: "", image: "worker-img/Nargiz.jpg", link: "" },
    { name: "", image: "worker-img/Seymur.jpg", link: "" },
    { name: "", image: "worker-img/Didem.jpg", link: "" },
    { name: "", image: "worker-img/Vagif.jpg", link: "" },
  ];
</script>

<div class="main">
  {#each WorkerList as worker}
    <WorkerItem name={worker.name} image={worker.image} link={worker.link} />
  {/each}
</div>
<img src="" alt="" />

<style>
  .main {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 10px;
    transition: 0.05s ease;
    max-width: 1700px;
    justify-content: center;
  }

  @media (max-width: 768px) {
    .main {
      justify-content: center;
    }
  }
</style>
