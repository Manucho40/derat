<template>
    <div class="services" id="services">
        <div class="espace-services">
            <h1>Services</h1>
            <p>Qu'est ce que nous offrons?</p>
        </div>
        <div class="cardServices">
                <CardServices />
                <CardServices />
                <CardServices />
        </div>
    </div>
</template>

<script>
import CardServices from './card-services.vue';
export default {
    components: { CardServices }
}
</script>

<style>
    .espace-services{
        display: flex;
        background-color: #ffff;
        flex-direction: column;
        padding: 20px;
        align-items: center;
    }
    .espace-services h1{
        font-size: 5rem;
    }
    .espace-services p {
        font-size: 2rem;
    }

    .espace-card{
        margin: auto;
    }
    .cardServices{
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
    }
</style>