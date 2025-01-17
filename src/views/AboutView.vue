<template>
  <navbar />

  <div class=" text-dark text-center mt-5">
    <div>
      <h2 class="fw-bold">Why should it be us?</h2>
    </div>

    <div class="container py-5 p-2" style="background-color: #f8f9fa;">
      <div class="container my-5 py-5">
        <div class="row align-items-center">
          <!-- Bagian Gambar -->
          <div class="col-md-6">
            <div class="image-container">
              <img src="/batik3.png" alt="Cover Batik" class="img-fluid rounded shadow-lg">
            </div>
          </div>
          <!-- Bagian Teks -->
          <div class="col-md-6">
            <div class="text-container">
              <h2 class="mb-4 fw-bold" style="color: #3a3a3a; font-size: 2rem;">
                Rumah Batik menyediakan batik tulis dan cap dengan desain yang memadukan tradisi dan
                modernitas.
              </h2>
              <p style="color: #555; font-size: 1.2rem; line-height: 1.8;">
                Kami juga menawarkan celana dan rok berbahan batik yang nyaman dan elegan. Setiap produk
                dibuat
                dengan perhatian terhadap detail dan kualitas, memberikan pengalaman istimewa mengenakan
                batik
                Indonesia.
              </p>
            </div>
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
import AppFooter from '@/components/AppFooter.vue';
import Navbar from '@/components/Navbar.vue';

export default {
  name: 'AboutView',
  components: {
    AppFooter,
    Navbar
  }
}
</script>

<style></style>