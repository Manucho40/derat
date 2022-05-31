<template>
    <div>
        <section class="header">
            <div class="divLogo">
                <img src="@/static/logo.png" alt="">
            </div>
            <div class="divNav">
                <div class="infos">
                    <span>support@yourdomain.tld</span>
                    <span>+6221.2002.2012</span>
                </div>
                <div>
                <b-navbar toggleable="lg" type="dark" variant="info">

                    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

                    <b-collapse id="nav-collapse" is-nav>

                    <!-- Right aligned nav items -->
                    <b-navbar-nav class="ml-auto">
                        <b-navbar-nav >
                             <b-nav-item href="#services">Services</b-nav-item>
                             <b-nav-item href="#produits">Produits</b-nav-item>
                             <b-nav-item href="#tarifs">Tarifs</b-nav-item>
                             <b-nav-item href="#">Infos</b-nav-item>
                        </b-navbar-nav>
                    </b-navbar-nav>
                    </b-collapse>
                </b-navbar>
                </div>
            </div>
        </section>
            <Nuxt />
    </div>
</template>

<script>
export default {

}
</script>

<style>
      body{
      background-color: #e4e8e8;
      
  }
.header{
    background-color: #ffffff;
    width: 100%;
    display: flex;
    justify-content: space-around;
    position: fixed;
    z-index: 1;
}
.divLogo{
    background-color: #002f47;
    width: 200px;
    margin-left: 200px;
    display: flex;
    align-items: center;
    padding: 20px;
}
.divLogo img {
    max-width: 175px;
    background-color: #002f47;
    margin: auto;
}

.divNav{
    background-color:#ffffff ;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    flex-grow: 1;
    margin-right: 200px;
}

.nav{
    display: flex;
    background-color: #ffffff;
    justify-content: flex-end;
    list-style-type: none;
    padding: 10px;
    margin-bottom: 0;
    margin-top: 30px;
}

.nav li{
    margin-right: 5px;
    border-right: 1px solid;
    padding: 5px;
}

.infos{
   background-color: #f5f7f2;
   width: 100%;
   display: flex;
   justify-content: flex-end;
   font-size: 20px;
}
.infos span{
    margin: 10px;
    
}

.menu{
    display: flex;
    flex-direction: column;
    width: 100%;
    margin: 0;
    padding: 0;
    

}

@media (max-width: 768px){
  .divLogo{
   width: 300px;
   padding: 0px;
   margin-left: 500px;
  }
  

  .infos{
      visibility: hidden;
  }
}

</style>