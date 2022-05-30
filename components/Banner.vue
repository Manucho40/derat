<template>
  <div class="banner">
      <div class="banner-text">
          <p>PROTEGER VOTRE MAISON</p>
          <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut elit tellus, luctus nec ullamcorper mattis, pulvinar dapibus leo.</span>
          <b-button variant="success">Button</b-button>
      </div>
      <div class="banner-img">
          <img src="@/static/img1.png" alt="">
      </div>
  </div>
</template>

<script>
export default {
   

}
</script>

<style>
   .banner{
       width: 100%;
       display: flex;
       justify-content: space-around;
       height: 90vh;
   }
   .banner-text{
       display: flex;
       flex-direction: column;
       justify-content: center;
   }
   .banner-text p{
       font-size: 4rem;
       font-weight: bold;
   }

</style>