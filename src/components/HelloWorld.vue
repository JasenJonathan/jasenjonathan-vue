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
          saya kebanyakan di rumah, jadi malas keluar<br>
          NEET<br>
          saya dulu ingin menjadi dokter tetapi tidak kuat melihat darah jadi berubah.
        </h3>
      </div>
      <div class="carousel-item">
        <div class="img-container">
          <img src="hobby.png">
        </div>
        <h2>
         <table class="table">
            <thead>
              <tr>
                <th scope="col">#</th>
                <th scope="col">What i do</th>
                <th scope="col">Achievement</th>
              </tr>
            </thead>
          <tbody>
            <tr>
              <th scope="row">1</th>
              <td>Game Design</td>
              <td>None</td>
            </tr>
            <tr>
              <th scope="row">2</th>
              <td>Game Programming</td>
              <td>None</td>
            </tr>
            <tr>
              <th scope="row">3</th>
              <td>Gaming</td>
              <td>None</td>
            </tr>
          </tbody>
        </table>
        </h2>
        
      </div>
      <div class="carousel-item">
        <div class="img-container">
          <img src="gear.png">
        </div>
        <h2>More About me</h2>
        <h2>Nama saya jasen jonathan, saya berumur 18 tahun</h2>
        <h2>Saya lahir pada tanggal 24 Januari 2003</h2>
        <h2>Tinggal di Jl. MP Mangkunegara No.04</h2>
        <h2>Email : jasenjonathan123@gmail.com</h2>
        <h2>No. Telp : 082246847270</h2>
        <button type="button" class="button">Contact Me</button>
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

