<script>
  import Subheader from "../../lib/Subheader.svelte";

  let pageTitle = 'Who we are'
</script>

<svelte:head><title>{pageTitle} • Mtt</title></svelte:head>
<div class="main">
  <Subheader pageTitle={pageTitle}/>
  <div class="hero">
    <img src="/dog.jpeg" alt="dog">
    <div class="text">
      <p>
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Vel, laborum hic quo iste aliquam alias sed rem odio voluptas odit saepe nobis natus necessitatibus nemo accusantium molestiae fugiat. Reprehenderit, quae commodi magni eaque accusantium quaerat ullam cupiditate ducimus repellendus, dolorum rerum eum quibusdam? Reprehenderit minima quaerat voluptatum veniam error, nostrum cumque, vel ducimus accusamus vitae quae consequuntur aliquid? Quis porro optio tempore enim, soluta nesciunt quam pariatur eligendi reiciendis necessitatibus blanditiis amet est, laborum, repellendus eveniet debitis quidem facilis praesentium nihil doloribus odit officiis. Exercitationem tempora id dolore! Eum sequi mollitia dicta repudiandae est a quia, consequuntur suscipit provident nobis.
      </p>
      <p>
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Vel, laborum hic quo iste aliquam alias sed rem odio voluptas odit saepe nobis natus necessitatibus nemo accusantium molestiae fugiat. Reprehenderit, quae commodi magni eaque accusantium quaerat ullam cupiditate ducimus repellendus, dolorum rerum eum quibusdam? Reprehenderit minima quaerat voluptatum veniam error, nostrum cumque, vel ducimus accusamus vitae quae consequuntur aliquid? Quis porro optio tempore enim, soluta nesciunt quam pariatur eligendi reiciendis necessitatibus blanditiis amet est, laborum, repellendus eveniet debitis quidem facilis praesentium nihil doloribus odit officiis. Exercitationem tempora id dolore! Eum sequi mollitia dicta repudiandae est a quia, consequuntur suscipit provident nobis.
      </p>
    </div>
  </div>  
</div>

<style>
  .main {
    display: flex;
    flex-direction: column;
    width: 100%;
  }
  .main img {
    width: 50%;
    height: 100%;
  }
  .hero {
    display: flex;
    flex-direction: row;
  }
  p {
    color: white;
    font-size: 2rem;
    margin: 0 20px;
  }
</style>