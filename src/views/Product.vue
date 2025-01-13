<template>

    <div>
        <navbar/>
    </div>

  <div class="text-center mt-5">
    <Batik/>
  </div>

  <div>
    <AppFooter/>
  </div>
  
</template>

<script>

import Batik from '@/components/Batik.vue';
import Navbar from '@/components/Navbar.vue';
import AppFooter from '@/components/AppFooter.vue';

export default {
    name: "ProductView",
    components: {
     Batik,
     Navbar,
     AppFooter
    }
}
</script>

<style>

</style>