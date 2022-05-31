<template>
  <div class="banner">
      <div class="banner-text p-3 animate__animated animate__fadeInRight animate__delay-2s">
          <p>PROTEGER <br> VOTRE MAISON</p>
          <span class="lead mb-5">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut elit tellus, luctus nec ullamcorper mattis, pulvinar dapibus leo.</span>
          <div>
              <b-button class="w-25 p-3" variant="success">OBTENIR UN DEVIS</b-button>
          </div>
      </div>
      <div class="banner-img animate__animated animate__fadeInLeft animate__delay-2s">
          <b-img src="@/static/img1.png" fluid alt="Responsive image"></b-img>
      </div>
  </div>
</template>

<script>
if (process.browser) { // Here we introduce... According to the environment wow.js
var {WOW} = require('wowjs')
}
export default {
      mounted() {
    this.$nextTick(() => {
  if (process.browser) { // On the page mounted In the life cycle Instantiate according to the environment WOW
  new WOW({animateClass: 'animate__animated'}).init()
  }
  });
  },

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
    @media (max-width: 768px){
        .banner{
           display: flex;
           flex-direction: column;
           align-items: center;
            height: 100vh;
            position: relative;
            /* top: 100px; */
        }
        .banner-text p{
            font-size: 2rem;
        }

        .banner-img img{
            width: 200px;
        }
    }
</style>