<script>
</script>

<section class="category">
  <h2 class="category-title">Choose Category</h2>
  <div class="category-section">
    <!-- {/* mapeo de las distintas categorias */} -->
    <article class="category-container">
      <div class="image-section-container">
        <img
          src="https://www.circalasvegas.com/wp-content/uploads/2021/01/MegaBar-72dpi.jpg"
          alt="imagen"
          class="rounded-image"
        />
        <div class="text-overlay">
          <h3 class="overlay">Restaurant</h3>
        </div>
      </div>
    </article>
    <article class="category-container">
      <div class="image-section-container">
        <img
          src="https://revistayoung.es/wp-content/uploads/2023/01/casino-en-linea.jpg"
          alt="imagen"
          class="rounded-image"
        />
        <div class="text-overlay">
          <h3 class="overlay">Online Casino</h3>
        </div>
      </div>
    </article>
    <article class="category-container">
      <div class="image-section-container">
        <img
          src="https://www.analyticsinsight.net/wp-content/uploads/2022/05/Online-Casino.jpg"
          alt="imagen"
          class="rounded-image"
        />
        <div class="text-overlay">
          <h3 class="overlay">Promotions</h3>
        </div>
      </div>
    </article>
    <article class="category-container">
      <div class="image-section-container">
        <img
          src="https://www.gamblingsites.com/app/uploads/2019/01/Support-for-Problem-Gambling-1200x771.png"
          alt="imagen"
          class="rounded-image"
        />
        <div class="text-overlay">
          <h3 class="overlay">Support</h3>
        </div>
      </div>
    </article>
  </div>
</section>

<style>
  .category {
    text-align: center;
  }

  .rounded-image {
    display: block;
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 10px;
    margin-top: -100px;
  }

  .text-overlay {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    color: #fff;
    z-index: 2;
  }

  .overlay {
    font-size: 1.4rem;
  }

  .category-section {
    text-align: center;
    width: 80%;
    max-width: 450px;
    margin: 0 auto;
    margin-top: 15px;
  }

  .category-container {
    margin-top: 10px;
  }

  .category-title {
    margin-top: 15px;
    color: rgb(255, 255, 255);
  }

  .image-section-container {
    position: relative;
    max-height: 125px;
    margin: 0 auto;
    overflow: hidden;
    border-radius: 10px;
  }

  .image-section-container::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.3);
    z-index: 1;
    border-radius: 10px;
  }

  .image-section-container :hover {
    color: #e3dcdc;
  }

  .category-section article :hover {
    cursor: pointer;
  }
</style>
