<template>

<div class="card" style="width: 18rem;">
    <img :src="'/batik/' + product.gambar" class="card-img-top" alt="...">
    <div class="card-body">
        <h5 class="card-title fw-bold">{{ product.nama }}</h5>
        <p class="card-text">{{ product.desk }}</p>
        <div class="d-flex justify-content-between">
            <button class="btn btn-secondary">Rp {{ product.harga }}</button>
            <router-link to="/product" class="btn btn-primary">Explore Now!</router-link>
        </div>
        <div class="d-flex justify-content-center mt-3">
            <router-link to="/checkout" class="btn btn-warning">CheckOut</router-link>
        </div>
    </div>
</div>




</template>

<script>
// import axios from 'axios';
export default {
    name: "BatikContent",
    props: ['product']
}
</script>

<style></style>