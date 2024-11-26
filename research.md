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
  .jmp-container {
    display: flex;
    align-items: flex-start;
    gap: 20px;
  }

  .jmp-content {
    flex: 2; /* Content takes up more space */
  }

  .jmp-carousel {
    flex: 1; /* Carousel takes up less space */
  }

  .carousel {
    position: relative;
    max-width: 100%; /* Fits container */
    overflow: hidden;
    border: 1px solid #ddd;
    border-radius: 8px;
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
    background: rgba(0, 0, 0, 0.5);
    color: white;
    border: none;
    padding: 5px;
    cursor: pointer;
  }
</style>

# Job Market Paper

<div class="jmp-container">
  
<!-- Left-hand side: Markdown content -->
<div class="jmp-content">

### *What do women want in a job? Household constraints, gender-biased decisions and the reservation wage gap*

Draft available here: [Dropbox link](https://www.dropbox.com/scl/fi/vcikrhj1dvwrig3jwfnvj/JMP_Kenza_Elass.pdf?rlkey=kncf3g3ofj1zgbz53vc098nuh&st=e6poxbut&dl=0)

<details>
<summary>Abstract</summary>
Recent explanations of the gender wage gap emphasize the role of gender differences in job search, yet the role of household constraints remains underexplored. This paper uses French administrative data to investigate how childcare constraints shape women’s reservation wage and job search strategies...
</details>

<details>
<summary>Presentations</summary>
<ul>
  <li>ECONtribute and C-SEB Design & Behavior Seminar at Cologne University</li>
  <li>Areena JMC Symposium</li>
</ul>
</details>

</div>

<!-- Right-hand side: Carousel -->
<div class="jmp-carousel">

<div class="carousel">
  <div class="carousel-images">
    <img src="https://raw.githubusercontent.com/elasskenza/website/main/assets/JMP/figure_2.png" alt="Slide 1">
    <img src="https://raw.githubusercontent.com/elasskenza/website/main/assets/JMP/figure_4.png" alt="Slide 2">
    <img src="https://raw.githubusercontent.com/elasskenza/website/main/assets/JMP/figure_5.png" alt="Slide 3">
    <img src="https://raw.githubusercontent.com/elasskenza/website/main/assets/JMP/figure_6.png" alt="Slide 4">
  </div>
  <button class="carousel-button prev">❮</button>
  <button class="carousel-button next">❯</button>
</div>

</div>
</div>

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

setInterval(nextImage, 5000); // 5 seconds per slide
</script>
