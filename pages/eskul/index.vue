<template>
  <div class="container">
    <h2 class="text-center mb-4">{{ getTitle() }}</h2>
    <div class="row">
      <div class="col">
        <div class="card">
          <img src="assets/img/bskt.jpg" class="card-img-top" alt="nama" />
          <div class="card-body">
            <h5 class="card-title">Basket</h5>
            <p class="card-text">Ekstrakurikuler olahraga Basket untuk meningkatkan keterampilan bermain bola basket.</p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="assets/img/seni.jpg" class="card-img-top" alt="nama" />
          <div class="card-body">
            <h5 class="card-title">Paduan suara</h5>
            <p class="card-text">'Ekstrakurikuler menyanyi bersama dalam kelompok untuk mempererat tali persaudaraan.',</p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="assets/img/futsal.jpg" class="card-img-top" alt="nama" />
          <div class="card-body">
            <h5 class="card-title">Futsal</h5>
            <p class="card-text">'Futsal adalah olahraga bola kecil yang dimainkan secara tim di lapangan mini.</p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="assets/img/paskibra.jpg" class="card-img-top" alt="nama" />
          <div class="card-body">
            <h5 class="card-title">Paskibra</h5>
            <p class="card-text">Paskibraka adalah singkatan dari Pasukan Pengibar Bendera Pusaka</p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="assets/img/pd.jpg" class="card-img-top" alt="nama" />
          <div class="card-body">
            <h5 class="card-title">Pencak silat</h5>
            <p class="card-text">Belajar seni bela diri tradisional Indonesia.</p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="assets/img/cinema.jpg" class="card-img-top" alt="nama" />
          <div class="card-body">
            <h5 class="card-title">Fotografi</h5>
            <p class="card-text">Mengembangkan kemampuan fotografi dan berkreasi dengan kamera.</p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="assets/img/laskar.jpg" class="card-img-top" alt="nama" />
          <div class="card-body">
            <h5 class="card-title">Laskar</h5>
            <p class="card-text">Laskar Pustaka adalah program yang diluncurkan oleh Lembaga Pemasyarakatan.</p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="assets/img/voly.jpg" class="card-img-top" alt="nama" />
          <div class="card-body">
            <h5 class="card-title">Voly</h5>
            <p class="card-text">permainan bola voli adalah permainan beregu yang menuntut kerjasama.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: "Daftar Ekstrakurikuler",
    };
  },
  methods: {
    getTitle() {
      return this.title;
    },
  },
};
</script>

<style scoped>
.container {
  margin-top: 10%;
}

h2 {
  font-size: 2rem;
  color: #424242;
}

.row {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}

.col {
  flex: 1 0 21%; /* Responsif: 4 kolom di desktop */
  min-width: 250px;
  margin-bottom: 20px;
}

.card {
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}

.card img {
  max-height: 200px;
  object-fit: cover;
  width: 100%;
}

.card-body {
  padding: 15px;
}

.card-title {
  font-size: 1.25rem;
  color: #333;
  margin-bottom: 10px;
}

.card-text {
  font-size: 1rem;
  color: #555;
  margin-bottom: 15px;
}

.btn {
  font-size: 1rem;
  padding: 8px 20px;
}

/* Responsivitas */
@media (max-width: 768px) {
  .row {
    justify-content: center;
  }

  .col {
    flex: 1 0 45%; /* 2 kolom di layar kecil */
  }
}

@media (max-width: 480px) {
  .col {
    flex: 1 0 100%; /* 1 kolom penuh pada layar ekstra kecil */
  }
}
</style>
