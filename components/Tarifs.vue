<template>
    <div id="tarifs">
        <Separateur :infoSection="infoSection" />
        <div class="tarifsCard mt-5">
            <div class="tarif-card card">
                    <h2>DERATISATION</h2>
                    <p class="lead ">Dératisation*</p>
                    <b-table striped hover :items="deratisation"></b-table>
            </div>
            <div class="tarif-card card">
                    <h2>DESINSECTISATION</h2>
                    <p class="lead ">Pulvérisation*</p>
                     <b-table striped hover :items="desinsectisation"></b-table>
            </div>
            <div class="tarif-card card">
                <h2>PUNAISE DE LIT</h2>
                <p class="lead ">Chimique/insecticide*</p>
                <b-table striped hover :items="punaise_de_lit"></b-table>   
            </div>
       
        </div>
    </div>
</template>

<script>
export default {
        data(){
        return {
            infoSection: {
            nomSection: "Tarifs",
            description: "Tarification de nos prestations"
        },
        punaise_de_lit: [
          { Superficie: '0 à 30 m2', Tarif_TTC: '170,00€' },
          { Superficie: '31 à 60 m2', Tarif_TTC: '180,00€' },
          { Superficie: '61 à 90 m2', Tarif_TTC: '200,00€' },
          { Superficie: '91 à 120 m2', Tarif_TTC: '220,00€' },
          { Superficie: '121 à 150 m2', Tarif_TTC: '240,00€' },
          { Superficie: '151 à 180 m2', Tarif_TTC: '260,00€' },
          { Superficie: '181 m2 ou plus', Tarif_TTC: 'Sur devis'}
        ],
        desinsectisation: [
          { Superficie: '0 à 30 m2', Tarif_TTC: '160,00€' },
          { Superficie: '31 à 60 m2', Tarif_TTC: '180,00€' },
          { Superficie: '61 à 90 m2', Tarif_TTC: '200,00€' },
          { Superficie: '91 à 120 m2', Tarif_TTC: '220,00€' },
          { Superficie: '121 à 150 m2', Tarif_TTC: '240,00€' },
          { Superficie: '151 à ou plus', Tarif_TTC: 'Sur devis' }
        ],
        deratisation: [
          { Superficie: '0 à 30 m2', Tarif_TTC: 'à partir de 139,00€' },
          { Superficie: '31 à 60 m2', Tarif_TTC: 'à partir de 159,00€' },
          { Superficie: '61 à 90 m2', Tarif_TTC: 'à partir de 179,00€' },
          { Superficie: '91 à 120 m2', Tarif_TTC: 'à partir de 199,00€' },
        ],
        }
    }
}
</script>

<style>
    .tarifsCard{
        display: flex;
        justify-content: center;
        margin: auto 100px;
        
    }

    .tarif-card{
        padding: 4em;
    }

    @media (max-width: 768px){
        .tarifsCard{
            display: flex;
            flex-direction: column;
            margin: auto 20px;
        }
        .tarif-card{
        padding: 1em;
        margin-bottom: 10px;
    }

    }
    
</style>