<template>
    <div class="services" id="services">
        <Separateur :infoSection="infoSection" />
        <div class="cardServices">
                <CardServices />
                <CardServices class="" />
                <CardServices class=""/>
                <CardServices class=""/>
                <CardServices class=""/>
                <CardServices class="" />
        </div>
    </div>
</template>

<script>
    import CardServices from './CardServices.vue'


export default {
    components: { CardServices },
 
    data(){
        return {
            infoSection: {
            nomSection: "Services",
            description: "Qu'est ce que nous offrons?"
        }
        }
    }
}
</script>

<style>


    .espace-card{
        margin: auto;
    }
    .cardServices{
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
    }
</style>