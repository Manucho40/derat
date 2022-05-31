<template>
        <div class="separateur">
            <h1>{{infoSection.nomSection}}</h1>
            <p>{{infoSection.description}}</p>
        </div>
</template>

<script>
export default {
    props:["infoSection"]
        
    
}
</script>

<style>
    .separateur{
        display: flex;
        background-color: #ffff;
        flex-direction: column;
        padding: 20px;
        align-items: center;
    }
    .separateur h1{
        font-size: 5rem;
    }
    .separateur p {
        font-size: 2rem;
    }
</style>