<style>
  /* General Styling */
  .button-container {
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
    margin-top: 10px;
  }

  /* Carousel Specific */
  .carousel {
    position: relative;
    max-width: 300px; /* Reduced size */
    margin: 0 auto;
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
    padding: 5px;
    cursor: pointer;
    border-radius: 5px;
  }

  .carousel-button:hover {
    background-color: rgba(0, 0, 0, 0.7);
  }

  /* Positioning Carousel and Content */
  .jmp-container {
    display: flex;
    gap: 20px; /* Space between abstract and carousel */
    align-items: flex-start;
  }

  .jmp-content {
    flex: 2; /* Take up more space than the carousel */
  }

  .jmp-carousel {
    flex: 1; /* Carousel takes up less space */
  }
</style>

<section>
  <h1>Research</h1>

  <!-- Job Market Paper Section -->
  <div class="jmp-container">
    <!-- Content Section -->
    <div class="jmp-content">
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
    </div>

    <!-- Carousel Section -->
    <div class="jmp-carousel">
      <div class="carousel">
        <div class="carousel-images">
          <img src="https://raw.githubusercontent.com/elasskenza/website/main/assets/JMP/figure_2.png" alt="Figure 2">
          <img src="https://raw.githubusercontent.com/elasskenza/website/main/assets/JMP/figure_4.png" alt="Figure 4">
          <img src="https://raw.githubusercontent.com/elasskenza/website/main/assets/JMP/figure_5.png" alt="Figure 5">
          <img src="https://raw.githubusercontent.com/elasskenza/website/main/assets/JMP/figure_6.png" alt="Figure 6">
          <img src="https://raw.githubusercontent.com/elasskenza/website/main/assets/JMP/figure_8.png" alt="Figure 8">
          <img src="https://raw.githubusercontent.com/elasskenza/website/main/assets/JMP/figure_9.png" alt="Figure 9">
          <img src="https://raw.githubusercontent.com/elasskenza/website/main/assets/JMP/figure_10.png" alt="Figure 10">
          <img src="https://raw.githubusercontent.com/elasskenza/website/main/assets/JMP/figure_11.png" alt="Figure 11">
        </div>
        <div class="carousel-buttons">
          <button class="carousel-button prev">❮</button>
          <button class="carousel-button next">❯</button>
        </div>
      </div>
    </div>
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
