<template>

    <div class="card" style="width: 18rem;">
        <img :src="'/batik/' + product.gambar" class="card-img-top" alt="...">
        <div class="card-body">
            <h5 class="card-title fw-bold">{{ product.nama }}</h5>
            <p class="card-text">{{ product.desk }}</p>
            <router-link to="/product" class="btn btn-primary float-right">Explore
                Now!</router-link>
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

<style>
</style>