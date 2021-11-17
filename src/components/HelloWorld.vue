<template>
  <div class="hello"></div>
  <div class="animation-area">
      <ul class="box-area">
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
      </ul>
  </div>
  <div id="carouselExampleDark" class="carousel carousel-dark slide" data-bs-ride="carousel">
    <div class="carousel-inner">
      <div class="carousel-item active">
        <div class="img-container">
            <img src="profile.jpg">
        </div>
          <h2>
            Hello my name is Jasen Jonathan
          </h2>
        <h3>
          saya seorang mahasiswa dari Universitas Multi Data Palembang.<br>
          18 tahun<br>
          NEET<br>
          beragama buddha
        </h3>
      </div>
      <div class="carousel-item">
        <div class="img-container">
          <img src="hobby.png">
        </div>
        
      </div>
      <div class="carousel-item">
        <div class="img-container">
          <img src="gear.png">
        </div>
      </div>
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleDark" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleDark" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

