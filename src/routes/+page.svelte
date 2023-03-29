<script>
  import Categories from "../lib/components/Categories.svelte";
</script>

<svelte:head>
  <title>Home</title>
  <meta name="description" content="EmpireCasino app" />
</svelte:head>

<section class="banner">
  <div class="banner-container">
    <div class="image-banner-container">
      <img
        src="https://a.cdn-hotels.com/gdcs/production199/d1463/cae57e13-2034-4ed6-bcfe-30fba0733f36.jpg"
        alt="imagen"
        class="rounded-image"
      />
      <button class="text-overlay">
        <h2 class="overlay">PLAY FOR FUN<br />PLAY SAFE</h2>
      </button>
    </div>
  </div>
</section>

  <Categories />

<style>
  .banner-container {
    width: 90%;
    margin: 0 auto;
    margin-top: 15px;
  }

  .image-banner-container {
    position: relative;
    max-height: 175px;
    margin: 0 auto;
    overflow: hidden;
    border-radius: 10px;
  }

  .image-banner-container::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.4);
    z-index: 1;
    border-radius: 10px;
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

  .image-banner-container :hover {
    cursor: pointer;
    color: #e3dcdc;
  }

  .overlay {
    font-size: 1.4rem;
  }
</style>
