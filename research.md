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

# Research

<!-- Start of reveal.js slides -->

<section data-markdown>
<script type="text/template">
# Job Market Paper

### *What do women want in a job? Household constraints, gender-biased decisions and the reservation wage gap*

##### Draft available upon request

- Using French administrative data to investigate gender-specific decisions in reservation wage gaps.
- 2018 childcare reform's effect on reservation wage and job search behavior.
- Findings: More affordable access to childcare allows women to target flexible jobs and secure stable employment.

### Presentations
- EEA-ESEM 2024, EALE 2024, Junior Economist Meeting 2024, ADRES 2023, AFSE 2023, etc.

</script>
</section>

<!-- Slide for a Picture -->
<section>
    <h2>Slide 1 - Placeholder Image</h2>
    <img src="https://via.placeholder.com/1024x768" alt="Placeholder Image 1" style="width:80%; height:auto;">
</section>

<!-- Slide for a Picture -->
<section>
    <h2>Slide 2 - Placeholder Image</h2>
    <img src="https://via.placeholder.com/1024x768" alt="Placeholder Image 2" style="width:80%; height:auto;">
</section>

<!-- Slide for a Picture -->
<section>
    <h2>Slide 3 - Placeholder Image</h2>
    <img src="https://via.placeholder.com/1024x768" alt="Placeholder Image 3" style="width:80%; height:auto;">
</section>

<!-- End of reveal.js slides -->

## Working Papers

### *Gender gaps in the urban wage premium*
With Cecilia García-Peñalosa & Christian Schluter - [Link to Working Paper](https://drive.google.com/file/d/1J18zTnQztCXFyi2CPf6kuWhTB35S_e0U/view)

<details>
  <summary>Abstract</summary>
    <p class="text-justify">
    Examines economic geography of gender wage gaps and urban wage premiums using French administrative data.
    </p>
</details>

<details>
  <summary>Presentations</summary>
  King’s Junior Research Day 2023, ADRES 2023, GRAPE 2023, etc.
</details>

### *Generative AI & Labor Market Discrimination*
With Germain Gauthier, Debora Nozza, Paola Profeta - [Link to Pre-analysis Plan](https://www.socialscienceregistry.org/trials/13538/history/220793)

<details>
  <summary>Abstract</summary>
    <p class="text-justify">
    Study of gender-stereotyped CVs produced by AI models and their discriminatory outcomes.
    </p>
</details>

<details>
  <summary>Presentations</summary>
  Dondena AI and Society Initiative Seminar at Bocconi University.
</details>

## Selected Work in Progress
- **Gender Norms and Child Development**, with Hélène Le Forner (CREM)
- **Changing the media narrative: the role of social movements**, with Caroline Coly (IEB) and Mahima Vasishth (Bocconi University)
- 

!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <meta
      name="viewport"
      content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no"
    />

    <title>Demo Portfolio</title>

    <link rel="stylesheet" href="dist/reset.css" />
    <link rel="stylesheet" href="dist/reveal.css" />
    <link rel="stylesheet" href="dist/theme/black.css" />

    <!-* Theme used for syntax highlighted code -->
    <link rel="stylesheet" href="plugin/highlight/monokai.css" />
  </head>
  <body>
    <div class="reveal">
      <div class="slides">
        <section>Unicorn slide<img src="assets/Bocconi.png" /></section>
        <section>Cupcake slide <img scr "assets/Selection_wage.jpg"></section>
      </div>
    </div>

    <script src="dist/reveal.js"></script>
    <script src="plugin/notes/notes.js"></script>
    <script src="plugin/markdown/markdown.js"></script>
    <script src="plugin/highlight/highlight.js"></script>
    <script>
      // More info about initialization & config:
      // * https://revealjs.com/initialization/
      // * https://revealjs.com/config/
      Reveal.initialize({
        hash: true,

        // Learn about plugins: https://revealjs.com/plugins/
        plugins: [RevealMarkdown, RevealHighlight, RevealNotes],
      });
    </script>
  </body>
</html>
