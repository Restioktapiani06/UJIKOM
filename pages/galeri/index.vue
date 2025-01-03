<template>
  <div class="container py-4">
    <h2 class="text-center mb-5">Galeri Sekolah</h2>
    <div class="gallery-grid">
      <!-- Kartu Galeri 1 -->
      <div class="card" data-bs-toggle="modal" data-bs-target="#lightbox1">
        <div class="img-wrapper">
          <img src="~assets/img/hari guru.jpg" class="card-img-top" alt="Kegiatan 1" />
        </div>
        <div class="card-body text-center">
          <p class="card-text">Upacara Hari Guru</p>
        </div>
      </div>

      <!-- Kartu Galeri 2 -->
      <div class="card" data-bs-toggle="modal" data-bs-target="#lightbox2">
        <div class="img-wrapper">
          <img src="~assets/img/upacara.jpg" class="card-img-top" alt="Prestasi 1" />
        </div>
        <div class="card-body text-center">
          <p class="card-text">Upacara Bendera</p>
        </div>
      </div>

      <!-- Kartu Galeri 3 -->
      <div class="card" data-bs-toggle="modal" data-bs-target="#lightbox3">
        <div class="img-wrapper">
          <img src="~assets/img/safty riding.jpg" class="card-img-top" alt="Safety-Ridding" />
        </div>
        <div class="card-body text-center">
          <p class="card-text">Safety-Ridding</p>
        </div>
      </div>

      <div class="card" data-bs-toggle="modal" data-bs-target="#lightbox3">
        <div class="img-wrapper">
          <img src="assets/img/1.jpeg" class="card-img-top" alt="Safety-Ridding" />
        </div>
        <div class="card-body text-center">
          <p class="card-text">RPL</p>
        </div>
      </div>

      <div class="card" data-bs-toggle="modal" data-bs-target="#lightbox3">
        <div class="img-wrapper">
          <img src="assets/img/2.jpeg" class="card-img-top" alt="Safety-Ridding" />
        </div>
        <div class="card-body text-center">
          <p class="card-text">RPL 4</p>
        </div>
      </div>

      <div class="card" data-bs-toggle="modal" data-bs-target="#lightbox3">
        <div class="img-wrapper">
          <img src="assets/img/4.jpeg" class="card-img-top" alt="Safety-Ridding" />
        </div>
        <div class="card-body text-center">
          <p class="card-text">RPL</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  margin-top: 10%;
}

h2 {
  font-weight: bold;
  color: #333;
}

/* Mengatur grid untuk card */
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr); /* 3 kolom */
  gap: 20px;
  justify-items: center;
}

.card {
  width: 100%;
  max-width: 300px; /* Membatasi lebar maksimal card */
  height: 100%;
  cursor: pointer;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  overflow: hidden;
  margin: 0 auto;
}

.img-wrapper {
  position: relative;
  padding-top: 75%; /* 4:3 Aspect Ratio */
  overflow: hidden;
}

.card-img-top {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.3s;
}

.card-img-top:hover {
  transform: scale(1.05);
}

.card-body {
  padding: 15px;
  background: #fff;
}

.card-text {
  margin: 0;
  font-size: 1rem;
  color: #333;
}

/* Responsivitas */
@media (max-width: 992px) {
  .gallery-grid {
    grid-template-columns: repeat(2, 1fr); /* 2 kolom di layar sedang */
  }
}

@media (max-width: 576px) {
  .gallery-grid {
    grid-template-columns: 1fr; /* 1 kolom di layar kecil */
  }

  .container {
    padding: 10px;
  }

  .card {
    margin-bottom: 15px;
  }
}
</style>
