<template>
   <div class="main">
      <Banner />
      <Services />
      <Produits />
      <Tarifs />
   </div>
</template>

<script>
import Tarifs from '../components/Tarifs.vue';
export default {
    name: "IndexPage",
    layout: "Header",
    components: { Tarifs }
}
</script>

<style>
   .main{
        position: relative;
        top: 100px;
    }
</style>
