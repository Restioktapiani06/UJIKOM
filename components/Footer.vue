<template>
  <div class="container my-5 bg-primary mt-5">
    <footer class="bg-primary">
      <div class="d-flex justify-content-center align-items-center">
        <a href="https://web.facebook.com/4smkn/?locale=id_ID&_rdc=1&_rdr#" class="btn btn-primary btn-lg btn-floating mx-2" style="background-color: #54456b">
          <i class="fab fa-facebook-f"></i>
        </a>
        <a href="https://www.youtube.com/channel/UC9WmS4sPok-9bAmRF1ZXrrg" class="btn btn-primary btn-lg btn-floating mx-2" style="background-color: #54456b">
          <i class="fab fa-youtube"></i>
        </a>
        <a href="#" class="btn btn-primary btn-lg btn-floating mx-2" style="background-color: #54456b">
          <i class="fab fa-instagram"></i>
        </a>
      </div>

      <!-- Copyright -->
      <div class="text-center text-white p-3 bg-primary mt-3">© 2025 Copyright:Resti Oktapiani</div>
    </footer>
  </div>
</template>

<script setup>
import "@fortawesome/fontawesome-free/css/all.min.css";
</script>

<style scoped>
footer {
  background-color: blue;
  width: 100%;
  margin-top: 10%;
}

.btn-floating {
  width: 50px;
  height: 50px;
  display: inline-flex;
  justify-content: center;
  align-items: center;
  border-radius: 50%;
  transition: transform 0.2s;
}

.btn-floating:hover {
  transform: scale(1.1);
}

.btn-floating i {
  font-size: 1.2rem;
  color: #fff;
}
</style>
