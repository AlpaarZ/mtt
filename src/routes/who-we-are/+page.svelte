<script>
  import Subheader from "../../lib/Subheader.svelte";

  let pageTitle = 'Who we are'
</script>

<svelte:head><title>{pageTitle} • Mtt</title></svelte:head>
<div class="main">
  <Subheader pageTitle={pageTitle}/>
  <div class="hero">
    <div class="content">
      <p>
        In the world of business and technology, we believe that our value proposition is to deliver trust. 
        Its been an incredible journey for us till date in sourcing quality candidates for the companies’ competitive recruitment needs. 
        As a modern day agency, we offer a strategic approach to recruiting by taking care of all business values by understanding your requirements and finding you suited candidates from various industries. 
        We diligently engage with you to understand your quest for talent and then connect you with the best professionals who have sound experience in their respective fields or industry.
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
  .hero {
    display: flex;
    flex-direction: row;
  }
  p {
    color: white;
    font-size: 2rem;
    font-weight: 600;
    text-align: left;
    line-height: 2.5rem;
    padding: 0 1rem 0 0;
  }
</style>