<script>
  import Subheader from "../../lib/Subheader.svelte";

  let pageTitle = "Contact us";
</script>

<svelte:head><title>{pageTitle} • Mtt</title></svelte:head>
<div class="main">
  <Subheader {pageTitle} />
  <div class="info">
    <p class="content">
      Baku, Azerbaijan <br> +99450 222 20 05 <br> +99450 231 08 04 only for HRCI
      issues/exams <br> Info@mtt.az <br> Recruitment@mtt.az
    </p>
    <div class="form">
      <input type="text" placeholder="Name" />
      <input type="text" placeholder="Email address" />
      <textarea placeholder="Your message..." />
      <button>Send message</button>
    </div>
  </div>
  
</div>

<style>
  .main {
    display: flex;
    flex-direction: column;
    width: 100%;
  }
  .info {
    display: flex;
    flex-direction: row;
  }
  .content {
    line-height: 24px;
  }
  .form {
    background-color: #373737;
    display: flex;
    flex-direction: column;

    padding: 1rem;
    border-radius: 10px;
  }
  .form input {
    border: none;
    margin-bottom: 1rem;
    font-size: 1.5rem;
  }
  .form textarea {
    font-family: "Roboto", sans-serif;
  }
</style>
