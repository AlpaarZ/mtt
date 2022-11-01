<script>
  import Subheader from "../../lib/Subheader.svelte";

  let pageTitle = "Digital tools in Recruitment and Talent Attraction";
</script>

<svelte:head><title>{pageTitle} • Mtt</title></svelte:head>
<div class="main">
  <Subheader {pageTitle} />
  <div class="video-card">
    <div class="text">
      <p>
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Voluptatum
        dicta, quis, eveniet, blanditiis labore et possimus dolore aperiam
        mollitia neque illo rem quod laborum? Sunt delectus quaerat ipsam
        excepturi ut enim ab rerum error repellat blanditiis velit, tenetur
        vitae nemo laboriosam perspiciatis incidunt provident aspernatur
        praesentium maiores cumque? Laudantium doloribus architecto, harum
        tempora nemo, provident aliquam enim molestiae ad animi, sint laborum
        accusamus in. Reprehenderit est libero optio explicabo, consectetur
        perspiciatis, incidunt perferendis consequuntur delectus quae, eveniet
        nihil aliquid esse culpa. In inventore quas quos veniam cum iste nemo
        eos sit, corrupti perspiciatis velit fugiat quisquam pariatur optio
        cupiditate? Magnam.
      </p>
      <a href="https://easyhire.me/" target="_blank" rel="noreferrer"
        ><button>Find out more</button></a
      >
    </div>
    <div class="video-container">
      <iframe
        src="https://www.youtube-nocookie.com/embed/98uKlKvIiOk?autoplay=1&mute=1&loop=1"
        title="Easyhire video"
        frameborder="0"
        autoplay="1"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      />
    </div>
  </div>
  <div class="card-container">
    <div class="card">
      <h1 class="title">Video screening</h1>
      <div class="content">
        <ul>
          <li>Interview scheduling and reminders</li>
          <li>Panel interviews</li>
          <li>Flexible question formats</li>
          <li>Recording sharing and collaboration</li>
          <li>Data-driven hiring decisions</li>
          <li>Automated Transcription</li>
        </ul>
      </div>
    </div>
    <div class="card">
      <h1 class="title">Applicant tracking system</h1>
      <div class="content">
        <ul>
          <li>Easily compare candidates to make faster decisions</li>
          <li>Know more about your candidates</li>
          <li>Keep all interview data in one place</li>
          <li>Measure your hiring success and improve</li>
        </ul>
      </div>
    </div>
    <div class="card">
      <h1 class="title">Advanced Job Board</h1>
      <div class="content">
        <ul>
          <li>Accept applications via mobile, web or Google Assistant</li>
          <li>Customize look and feel</li>
          <li>Advertise on 3rd party sites</li>
          <li>Automate pre-screening</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<style>
  .main {
    display: flex;
    flex-direction: column;
    width: 100%;
  }
  .video-card {
    border-radius: 10px;
    padding: 2rem;
    flex-grow: 1;
    margin: 0 2rem 1rem 2rem;
    display: flex;
    flex-direction: row;
  }
  @media (max-width: 768px) {
    .video-card {
      flex-direction: column-reverse;
    }
  }
  .video-card .text {
    flex: 1;
    font-size: 1.5rem;
    flex-direction: column;
  }
  .video-card .text button {
    background-color: #373737;
    padding: 20px;
    border: none;
    color: white;
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
  .video-card .text button:active {
    opacity: 0.8;
  }
  .video-card .video-container {
    position: relative;
    overflow: hidden;
    width: 100%;
    padding-top: 56.25%;
    flex-grow: 0;
  }
  .video-container iframe {
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    width: 100%;
    height: 100%;
  }
  .card-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    gap: 1rem;
  }
  .card {
    width: 300px;
    text-align: left;
    border-radius: 10px;
    padding: 2rem;
    display: flex;
    flex-direction: column;
    gap: 1rem;

    background-color: #262626;
  }
  .card ul {
    line-height: 32px;
    list-style: disc;
  }
  h1 {
    font-size: 2rem;
    line-height: 36px;
    font-weight: 600;
  }
  .card .content {
    line-height: 24px;
  }
  @media (max-width: 768px) {
    .card-container {
      justify-content: center;
    }
    iframe {
      width: 300px;
      height: 200px;
    }
  }
</style>
