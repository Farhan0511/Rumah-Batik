<template>
  <div>
    <NavbarVue />
  </div>

  <div class="container py-5">
    <div class="row d-flex align-items-center">
      <!-- Konten Teks -->
      <div class="col-md-6 mb-4 mb-md-0">
        <div class="content-text">
          <h2 class="display-4 mb-3">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident excepturi magni facere!
          </h2>
          <p class="lead">
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laudantium, alias?
          </p>
        </div>
      </div>

      <!-- Gambar -->
      <div class="col-md-6">
        <img src="/batik3.png" alt="Cover Batik" class="img-fluid rounded shadow-sm">
      </div>
    </div>
  </div>
</template>

<script>
import NavbarVue from '@/components/Navbar.vue'

export default {
  name: 'HomeView',
  components: {
    NavbarVue,
  },
}
</script>

<style scoped>

h2 {
  font-size: 2rem;
  font-weight: 600;
}

p {
  font-size: 1.2rem;
  color: #555;
}

</style>

