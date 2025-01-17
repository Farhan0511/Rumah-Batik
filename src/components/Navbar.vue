<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-light" style="background-color: #f8f9fa;">
      <div class="container d-flex justify-content-between align-items-center">
        <!-- Logo dan Brand -->
        <div href="/" class="d-flex align-items-center">
          <img src="/batik2.png" alt="Rumah Batik" class="me-2"
            style="width: 120px; height: 80px; object-fit: cover;  text-decoration: none">

          <RouterLink class="navbar-brand fs-4 fw-bold text-black" to="/">Rumah Batik</RouterLink>

        </div>

        <!-- Toggler untuk mobile -->
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
          aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>

        <!-- Menu Navigasi -->
        <div class="collapse navbar-collapse justify-content-center" id="navbarNav">
          <ul class="navbar-nav">
            <!-- Home -->
            <li class="nav-item">
              <RouterLink class="nav-link fs-5 text-dark fw-semibold" to="/" style="text-decoration: none;">Home
              </RouterLink>
            </li>

            <!-- About -->
            <li class="nav-item">
              <RouterLink class="nav-link fs-5 text-dark fw-semibold" to="/about" style="text-decoration: none;">About
              </RouterLink>
            </li>

            <!-- Product -->
            <li class="nav-item">
              <RouterLink class="nav-link fs-5 text-dark fw-semibold" to="/product" style="text-decoration: none;">
                Product</RouterLink>
            </li>

            
          </ul>
        </div>

        <form class="d-flex" role="search">
          <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
          <RouterLink class="nav-link fs-5 text-dark fw-semibold" to="/checkout" style="text-decoration: none;">
            CheckOut</RouterLink>

          <!-- <div>
            <box-icon name='cart'></box-icon>

          </div> -->
        </form>
      </div>
    </nav>
  </div>




</template>

<script>
export default {
  name: 'NavbarVue'
}
</script>

<style></style>