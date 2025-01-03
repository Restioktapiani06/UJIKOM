<template>
  <div>
    <nav class="navbar">
      <div class="logo">
        <img src="~/assets/img/logo.jpg" alt="Logo Sekolah" />
        <div class="logo-text">
          SMKN 4 TASIKAMALAYA<br />
          Jl. Depok, Sukamenak, Kec. Purbaratu, Kab. Tasikmalaya, Jawa Barat 46196
        </div>
      </div>
      <div class="menu-toggle" @click="toggleMenu">
        <div class="bar"></div>
        <div class="bar"></div>
        <div class="bar"></div>
      </div>
      <ul :class="{ active: isMenuOpen }">
        <li><NuxtLink to="/">BERANDA</NuxtLink></li>
        <li><NuxtLink to="./profil">PROFIL</NuxtLink></li>
        <li><NuxtLink to="./jurusan">JURUSAN</NuxtLink></li>
        <li><NuxtLink to="./eskul">EKSTRAKULIKULER</NuxtLink></li>
        <li><NuxtLink to="/galeri">GALERI</NuxtLink></li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isMenuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
  },
};
</script>

<style scoped>
.navbar {
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #44abf0;
  color: #fff;
  padding: 1rem;
  flex-wrap: wrap;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1000;
}

.logo {
  display: flex;
  align-items: center;
  gap: 1rem;
}

.logo img {
  width: 50px;
  height: 50px;
  object-fit: contain;
}

.logo-text {
  font-size: 0.9rem;
  line-height: 1.4;
}

ul {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
  align-items: center;
}

li {
  margin-right: 20px;
}

li:last-child {
  margin-right: 0;
}

a {
  color: #fff;
  text-decoration: none;
  padding: 0.5rem;
  display: block;
  transition: color 0.3s;
}

a:hover {
  color: #ccc;
}

.menu-toggle {
  display: none;
  flex-direction: column;
  cursor: pointer;
  padding: 5px;
}

.bar {
  width: 25px;
  height: 3px;
  background-color: #fff;
  margin: 2px 0;
  transition: 0.3s;
}

@media (max-width: 768px) {
  .navbar {
    padding: 1rem 0.5rem;
  }

  .logo {
    font-size: 0.8rem;
  }

  .logo img {
    width: 40px;
    height: 40px;
  }

  .menu-toggle {
    display: flex;
  }

  ul {
    display: none;
    width: 100%;
    flex-direction: column;
    text-align: center;
    padding: 1rem 0;
  }

  ul.active {
    display: flex;
  }

  li {
    margin: 10px 0;
  }

  a {
    padding: 0.5rem 1rem;
  }
}

@media (max-width: 576px) {
  .logo {
    flex-direction: column;
    align-items: flex-start;
    gap: 0.5rem;
  }

  .logo-text {
    font-size: 0.8rem;
  }
}
</style>
