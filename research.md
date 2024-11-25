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
  /* General Styling */
  summary {
    font-weight: bold;
    cursor: pointer;
    padding: 10px;
    background-color: #2a5866;
    color: white;
    border: 1px solid #001f3f;
    border-radius: 5px;
    width: fit-content;
    transition: background-color 0.3s ease;
  }

  summary:hover {
    background-color: #001a35;
  }

  details {
    margin-bottom: 15px;
  }

  details[open] summary {
    background-color: #001a35;
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
    margin-top: 10px;
  }

  iframe {
    width: 100%;
    height: 80vh;
    border: none;
  }

  hr {
    border: none;
    border-top: 1px solid #ccc;
    margin: 20px 0;
  }

  h1 {
    margin-top: 40px;
    font-size: 2em;
    text-align: center;
  }

  h2, h3, h4 {
    margin-top: 30px;
  }

  /* Rotating Carousel Styles */
  .carousel {
    position: relative;
    max-width: 800px;
    margin: 20px auto;
    overflow: hidden;
    border: 2px solid #ccc;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  }

  .carousel-images {
    display: flex;
    transition: transform 0.5s ease-in-out;
  }

  .carousel img {
    width: 100%;
    flex-shrink: 0;
  }

  .carousel-buttons {
    position: absolute;
    top: 50%;
    width: 100%;
    display: flex;
    justify-content: space-between;
    transform: translateY(-50%);
  }

  .carousel-button {
    background-color: rgba(0, 0, 0, 0.5);
    color: white;
    border: none;
    padding: 10px;
    cursor: pointer;
    border-radius: 5px;
  }

  .carousel-button:hover {
    background-color: rgba(0, 0, 0, 0.7);
  }
</style>

<section>
  <h1>Research</h1>

  <!-- Rotating Picture Carousel -->
  <div class="carousel">
    <div class="carousel-images">
      <img src="https://via.placeholder.com/800x400?text=Image+1" alt="Image 1">
      <img src="https://via.placeholder.com/800x400?text=Image+2" alt="Image 2">
      <img src="https://via.placeholder.com/800x400?text=Image+3" alt="Image 3">
    </div>
    <div class="carousel-buttons">
      <button class="carousel-button prev">❮</button>
      <button class="carousel-button next">❯</button>
    </div>
  </div>

  <h2>Job Market Paper</h2>
  <h3><i>What do women want in a job? Household constraints, gender-biased decisions, and the reservation wage gap</i></h3>
  <p>Draft available here: <a href="https://www.dropbox.com/scl/fi/vcikrhj1dvwrig3jwfnvj/JMP_Kenza_Elass.pdf?rlkey=kncf3g3ofj1zgbz53vc098nuh&st=e6poxbut&dl=0" target="_blank">Dropbox link</a></p>

  <div class="button-container">
    <details>
      <summary>Abstract</summary>
      <p class="text-justify">
        Recent explanations of the gender wage gap emphasize the role of gender differences in job search, yet the role of household constraints remains underexplored...
      </p>
    </details>

    <details>
      <summary>Presentations</summary>
      <ul>
        <li>ECONtribute and C-SEB Design & Behavior Seminar at Cologne University</li>
        <li>Areena JMC Symposium</li>
      </ul>
    </details>
  </div>
</section>

<script>
  const carouselImages = document.querySelector('.carousel-images');
  const images = document.querySelectorAll('.carousel img');
  const prevButton = document.querySelector('.carousel-button.prev');
  const nextButton = document.querySelector('.carousel-button.next');

  let currentIndex = 0;

  function updateCarousel() {
    const width = images[0].clientWidth;
    carouselImages.style.transform = `translateX(-${currentIndex * width}px)`;
  }

  function nextImage() {
    currentIndex = (currentIndex + 1) % images.length;
    updateCarousel();
  }

  function prevImage() {
    currentIndex = (currentIndex - 1 + images.length) % images.length;
    updateCarousel();
  }

  nextButton.addEventListener('click', nextImage);
  prevButton.addEventListener('click', prevImage);

  // Auto-rotate every 3 seconds
  setInterval(nextImage, 3000);
</script>
