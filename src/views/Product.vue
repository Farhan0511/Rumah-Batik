<template>

  <div>
    <navbar />

    <div class="container">
      <div class="row mt-5">
        <div class="col">
          <h2 class="text-center">Our Collection</h2>
        </div>
        <div class="row row-cols-1 row-cols-md-4 g-4">
          <div class="col text-center" v-for="product in products" :key="product.id">
            <Batik :product="product" />
          </div>
        </div>
      </div>
    </div>
  </div>

  <div>
    <AppFooter />

  </div>

</template>

<script>

import Navbar from '@/components/Navbar.vue';
import Batik from '@/components/Batik.vue';
import axios from 'axios';
import AppFooter from '@/components/AppFooter.vue';

export default {
  name: "ProductView",
  components: {
    Navbar,
    Batik,
    AppFooter
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
    axios.get('http://localhost:3000/products')
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

<style></style>