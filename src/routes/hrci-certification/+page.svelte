<script>
  import Subheader from "../../lib/Subheader.svelte";

  let pageTitle = "HRCI Certification Preparation Provider";
</script>

<svelte:head><title>{pageTitle} • Mtt</title></svelte:head>
<div class="main">
  <Subheader {pageTitle} />

  <p class="content">Since 2018 More Than Trust LLC became an HRCI Certification Preparation
    Provider for the Associate Professional in Human Resources – International™
    (aPHRi™), Professional in Human Resource – International ™ (PHRi™) & Senior
    Professional in Human Resource – International™ (SPHRi™) From now on we are
    here to support HR professionals on the road to career and business success
    through certification with HR Certification Institute® (HRCI®) — the world’s
    most recognized credentials for HR professionals. Applying us you may purchase
    Preparation and Exam for aPHRi, PHRi, and SPHRi No need to travel abroad to
    get most recognized credentials for HR professionals! Everything is now
    possible right here – Baku, Azerbaijan. For details please contact us: Email:
    info@mtt.az Phone: +99450 231 08 04 *The HR Certification Institute® (HRCI®)
    does not endorse any particular preparation program or offering. We encourage
    prospective certification holders to use a variety of resources that reflect
    their learning styles and needs. Purchasing a certification product is NOT
    required and HRCI does not guarantee that an individual will pass based on the
    purchase of a certification preparation product. *The red-and-purple HR
    design, HR CERTIFICATION INSTITUTE, aPHRi, PHRi, and SPHRi are trademarks of
    registered trademarks of Human Resource Certification Institute, Inc. in the
    U.S. and other countries. Used Under License.
  </p>
  <div class="card-container">
    <a class="card" href="pdfs/Cooperation-terms-2022.pdf" target="_blank">Cooperation Terms</a>
    <a class="card" href="pdfs/Exam-Preparation-Course.pdf" target="_blank">Information on Exam Preparation Course</a>
  </div>  
</div>

<style>
  .main {
    display: flex;
    flex-direction: column;
    width: 100%;
  }
  .content {
    padding: 1rem 0;
    line-height: 24px;
  }
  .card-container {
    display: flex;
    flex-wrap: wrap;
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

    background-color: #373737;
  }
</style>
