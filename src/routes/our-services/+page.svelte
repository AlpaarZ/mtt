<script>
  import Subheader from "../../lib/Subheader.svelte";

  let pageTitle = "Our services";
</script>

<svelte:head><title>{pageTitle} • Mtt</title></svelte:head>
<div class="main">
  <Subheader {pageTitle} />
  <div class="card-container">
    <div class="card">
      <h1 class="title">Recruitment and Executive Search</h1>
      <div class="content">
        “Right people, right place, right time” – old, but gold! We provide
        professional recruitment services (using professional assessment tools
        of SHL); search for unique specialists and head hunting. Just show whom
        you want and we will bring them on board.
      </div>
    </div>
    <div class="card">
      <h1 class="title">HR Audit</h1>
      <div class="content">
        Internal Audit of all HR processes, ready solutions and support in
        implementation:
        <ul>
          <li>Performance Management</li>
          <li>Organizational Development</li>
          <li>Grading system</li>
        </ul>
      </div>
    </div>
    <div class="card">
      <h1 class="title">Your Personal Brand</h1>
      <div class="content">
        «Your brand is what people say about you when you leave the room» — Jeff
        Bezos<br /><br />
        We will support you to create your personal brand.
        <ul>
          <li>CV creation</li>
          <li>Techniques of professional interview preparation</li>
          <li>Mock Interview</li>
          <li>Personality Tests</li>
          <li>Feedback</li>
          <li>Development Planning</li>
        </ul>
      </div>
    </div>
    <div class="card">
      <h1 class="title">Business Consulting</h1>
      <div class="content">
        We’re here to ensure that your business needs are fully covered and each
        time supported by Professionals and ready to support you in:

        <ul>
          <li>Finance and Accounting</li>
          <li>Advanced Analytics</li>
          <li>Strategy</li>
          <li>Business development</li>
          <li>Change management</li>
          <li>Project management</li>
          <li>Hotel management</li>
          <li>Information Technology</li>
        </ul>
      </div>
    </div>
  </div>

  <h1 class="training">Trainings</h1>

  <div class="card-container">
    <div class="card">
      <h1 class="title">Marketing</h1>
      <div class="content">
        <ul>
          <li>Strategy</li>
          <li>Analytics</li>
          <li>Digital</li>
          <li>Marketing Communications</li>
        </ul>
      </div>
    </div>
    <div class="card">
      <h1 class="title">Sales</h1>
      <div class="content">
        <ul>
          <li>Retail</li>
          <li>Franchise</li>
          <li>Online sales</li>
          <li>Telesales</li>
          <li>Corporate Sales</li>
          <li>HR as a Business Partner</li>
        </ul>
      </div>
    </div>
    <div class="card">
      <h1 class="title">Skills</h1>
      <div class="content">
        <ul>
          <li>Scrum/Agile/Kanban</li>
          <li>Project Management</li>
          <li>Conflict Management</li>
          <li>Excel</li>
          <li>Negotiation Skills</li>
          <li>Leadership</li>
          <li>Presentation Skills</li>
          <li>Coaching skills</li>
        </ul>
      </div>
    </div>
    <div class="card">
      <h1 class="title">Psychology</h1>
      <div class="content">
        <ul>
          <li>The clues of working with generations Y&Z</li>
          <li>Decoding and Incorporating Happiness</li>
          <li>Happiness self-sabotage</li>
          <li>Happiness at work</li>
          <li>Developing a leadership that helps increase team’s happiness and productivity</li>
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
  .card-container {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    justify-content: space-around;
  }
  @media (max-width: 768px)
  {
    .card-container {
      justify-content: center;
    }
    .training {
      text-align: center;
    }
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
  .training {
    font-size: 36px;
    font-weight: 200;
    padding: 1rem 0;
  }
</style>
