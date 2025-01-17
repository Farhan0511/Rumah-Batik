<template>
  <div class="">
    <NavbarVue />
  </div>

  <div class="container py-5 ">
    <div class="row align-items-center justify-content-between">
      <!-- Konten Teks -->
      <div class="col-md-6 text-md-start text-center mb-4 mb-md-0 ">
        <div class="content-text">
          <h2 class="display-4 fw-bold text-primary mb-3">
            Discover the Beauty of Batik
          </h2>
          <p class="lead text-secondary mb-4">
            Explore the rich cultural heritage of Batik art. Each pattern tells a unique story crafted with love and
            tradition.
          </p>
          <div>
            <router-link to="/product" class="btn btn-primary float-right">Explore
              Now!</router-link>
          </div>
        </div>
      </div>

      <!-- Gambar -->
      <div class="col-md-6">
        <div class="">
          <img src="/batik3.png" alt="Cover Batik" class="img-fluid rounded shadow-lg w-100">
        </div>
      </div>
    </div>
  </div>


  <!-- Component Batik -->
  <div class="container mt-5">
    <h2 class="text-center mb-4">Our Batik Collection</h2>
    <div class="row row-cols-1 row-cols-md-4 g-4 justify-content-center">
      <div class="col d-flex justify-content-center" v-for="product in products" :key="product.id">
        <BatikVue :product="product" />
      </div>
    </div>
  </div>

  <div>
    <deskripsi />
  </div>

  <div>
    <Location />
  </div>

  <div>
    <AppFooter />
  </div>

</template>

<script>
import NavbarVue from '@/components/Navbar.vue'
import BatikVue from '@/components/Batik.vue'
import Deskripsi from '@/components/Deskripsi.vue'
import AppFooter from '@/components/AppFooter.vue'
import Location from '@/components/Location.vue'
import axios from 'axios'

export default {
  name: 'HomeView',
  components: {
    NavbarVue,
    BatikVue,
    Deskripsi,
    AppFooter,
    Location
  },
  data() {
    return {
      products: []
    }
  },
  methods: {
    setProduct(data) {
      this.products = data
    }
  },
  mounted() {
    axios.get('http://localhost:3000/best-products')
      .then((response) => {
        // handle success
        this.setProduct(response.data);
      })
      .catch((error) => {
        // handle error
        console.log("Gagal :", error);
      });
  }

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
