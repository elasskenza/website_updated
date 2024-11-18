---
title: Research
layout: page
permalink: /research/
elements:
  - content
  - css
  - formatting
  - html
  - markup  
---

<style>
  summary {
    font-weight: bold;
    cursor: pointer;
    padding: 10px;
    background-color: #2a5866; /* Navy background */
    color: white; /* White text */
    border: 1px solid #001f3f;
    border-radius: 5px;
    width: fit-content;
  }

  summary:hover {
    background-color: #001a35; /* Slightly darker navy on hover */
  }

  details {
    margin-bottom: 15px;
  }

  details[open] summary {
    background-color: #001a35; /* Change background when open */
  }

  .text-justify {
    text-align: justify;
    padding: 10px;
    background-color: #f9f9f9;
    border-left: 4px solid #ccc;
    margin-top: 10px;
    border-radius: 3px;
  }

  .button-container {
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
  }

  @media (max-width: 600px) {
    .button-container {
      flex-direction: column;
    }
  }

  h1 {
    margin-top: 40px;
  }

  section {
    margin-top: 40px;
  }

  .page-title {
    text-align: center;
    font-style: normal;
  }
</style>


 ---
layout: page
permalink: /research/
elements:
  - content
  - css
  - formatting
  - html
  - markup  
---

<style>
  summary {
    font-weight: bold;
    cursor: pointer;
    padding: 10px;
    background-color: #2a5866; /* Navy background */
    color: white; /* White text */
    border: 1px solid #001f3f;
    border-radius: 5px;
    width: fit-content;
  }

  summary:hover {
    background-color: #001a35; /* Slightly darker navy on hover */
  }

  details {
    margin-bottom: 15px;
  }

  details[open] summary {
    background-color: #001a35; /* Change background when open */
  }

  .text-justify {
    text-align: justify;
    padding: 10px;
    background-color: #f9f9f9;
    border-left: 4px solid #ccc;
    margin-top: 10px;
    border-radius: 3px;
  }

  /* Ensures buttons (details) are aligned side by side */
  .button-container {
    display: flex;
    gap: 10px; /* Adds spacing between buttons */
    flex-wrap: wrap; /* Allows buttons to wrap if the screen is small */
  }

  /* Optional: Adjust for smaller screens */
  @media (max-width: 600px) {
    .button-container {
      flex-direction: column;
    }
  }

  /* Add vertical spacing before h1 */
  h1 {
    margin-top: 40px; /* Adds vertical spacing before h1 */
  }

  /* Add margin to a specific div or section containing the header */
  section {
    margin-top: 40px; /* Adds space before sections */
  }

  /* Center the specific page title with a class */
  .page-title {
    text-align: center; /* Centers the title */
    font-style: normal; /* Removes the italic style */
  }

  iframe {
    width: 100%;
    height: 80vh;
    border: none;
  }
</style>

<section>
  <h1 class="page-title">Research</h1>

  <h2>Job Market Paper</h2>

  <h3><i>What do women want in a job? Household constraints, gender-biased decisions and the reservation wage gap</i></h3>
  <p>Draft available here: <a href="https://www.dropbox.com/scl/fi/vcikrhj1dvwrig3jwfnvj/JMP_Kenza_Elass.pdf?rlkey=kncf3g3ofj1zgbz53vc098nuh&st=e6poxbut&dl=0" target="_blank">Dropbox link</a></p>

  <div class="button-container">
    <details>
      <summary>Abstract</summary>
      <p class="text-justify">
        Recent explanations of the gender wage gap emphasize the role of gender differences in job search, yet the role of household constraints remains underexplored. This paper uses French administrative data to investigate the importance of gender-specific decisions in the reservation wage gap, and specifically how household constraints shape women's reservation wage strategies...
      </p>
    </details>

    <details>
      <summary>Presentations</summary>
      <ul>
        <li>ECONtribute and C-SEB Design & Behavior Seminar at Cologne University</li>
        <li>Areena JMC Symposium</li>
        <li>EEA-ESEM 2024</li>
        <li>EALE 2024</li>
        <!-- More entries here -->
      </ul>
    </details>

    <details>
      <summary>Paper</summary>
      <div>
        <iframe src="../assets/JMP_Kenza_Elass.pdf">
          This browser does not support PDFs. Please download the PDF to view it:
          <a href="../assets/JMP_Kenza_Elass.pdf">Download PDF</a>.
        </iframe>
      </div>
    </details>
  </div>

  <br>
  <hr>

  <h2>Other Writing - General Audience</h2>

  <h3><i>Threat or opportunity? The impact of AI on women</i></h3>
  <p>With Paola Profeta (Bocconi University)</p>

  <div class="button-container">
    <details>
      <summary>Abstract</summary>
      <p class="text-justify">
        The adoption of AI in various sectors has led to changes that present both opportunities and challenges for gender equality. Although AI appears to be less biased than human decision-makers...
      </p>
    </details>

    <details>
      <summary>Paper</summary>
      <div>
        <iframe src="../assets/pdf/Elass_profeta_AI_Gender.pdf">
          This browser does not support PDFs. Please download the PDF to view it:
          <a href="../assets/pdf/Elass_profeta_AI_Gender.pdf">Download PDF</a>.
        </iframe>
      </div>
    </details>
  </div>

  <div>
    <h4>Communication</h4>
    <a href="https://www.repubblica.it/dossier/economia/top-story/2024/11/11/news/ia_opportunita_e_minaccia_per_l_uguaglianza_di_genere-423611448/" target="_blank">La Repubblica</a>
  </div>
</section>

