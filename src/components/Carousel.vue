<template>
  <div
    id="carouselExampleCaptions"
    class="carousel slide"
    data-bs-ride="carousel"
  >
    <div class="carousel-indicators home__carousel-indicators">
      <button
        type="button"
        data-bs-target="#carouselExampleCaptions"
        data-bs-slide-to="0"
        class="active"
        aria-current="true"
        aria-label="Slide 1"
      ></button>
      <button
        type="button"
        data-bs-target="#carouselExampleCaptions"
        data-bs-slide-to="1"
        aria-label="Slide 2"
      ></button>
      <button
        type="button"
        data-bs-target="#carouselExampleCaptions"
        data-bs-slide-to="2"
        aria-label="Slide 3"
      ></button>
    </div>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="../assets/img/slide.png" class="d-block w-100" alt="" />
        <div class="carousel-caption d-none d-md-block">
          <h5 class="home__carousel-title">120 Anastasia Avenue, Coral Gables</h5>
          <p class="home__carousel-subtitle">$625,000</p>
          <button class="home__carousel-btn">MORE INFO</button>
        </div>
      </div>
      <div class="carousel-item">
        <img src="../assets/img/slide2.png" class="d-block w-100" alt="" />
        <div class="carousel-caption d-none d-md-block">
          <h5 class="home__carousel-title">120 Anastasia Avenue, Coral Gables</h5>
          <p class="home__carousel-subtitle">$625,000</p>
          <button class="home__carousel-btn">MORE INFO</button>
        </div>
      </div>
      <div class="carousel-item">
        <img src="../assets/img/slide.png" class="d-block w-100" alt="" />
        <div class="carousel-caption d-none d-md-block">
          <h5 class="home__carousel-title">120 Anastasia Avenue, Coral Gables</h5>
          <p class="home__carousel-subtitle">$625,000</p>
          <button class="home__carousel-btn">MORE INFO</button>
        </div>
      </div>
    </div>
    <button
      class="carousel-control-prev"
      type="button"
      data-bs-target="#carouselExampleCaptions"
      data-bs-slide="prev"
    >
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button
      class="carousel-control-next"
      type="button"
      data-bs-target="#carouselExampleCaptions"
      data-bs-slide="next"
    >
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
  </div>
</template>

<style lang="scss">
.home {
  &__carousel-indicators {
    bottom: 250px;
  }
  &__carousel-title {
    font-family: 'Raleway', sans-serif;
    font-weight: 700;
    font-size: 48px;
  }
  &__carousel-subtitle {
    font-family: 'Montserrat', sans-serif;
    font-weight: 300;
    font-size: 36px;
  }
  &__carousel-btn {
    font-family: 'Raleway', sans-serif;
    font-weight: 700;
    font-size: 16px;

    padding: 12px;
    color: #fff;
   background: rgba(255, 255, 255, 0.3);
    border: none;
    border-radius: 5%;
  }
}
</style>