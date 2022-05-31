<template>
   <div id="produits">
       <Separateur :infoSection="infoSection" />
       <b-container class="mt-5 mb-5">
    <b-card-group deck>
    <b-card title="Fumigateur diffuseur insecticides hydro-réactif curatif choc" img-src="https://picsum.photos/300/300/?image=41" img-alt="Image" img-top>
      <b-card-text>
        This is a wider card with supporting text below as a natural lead-in to additional content.
        This content is a little bit longer.
      </b-card-text>
      <template #footer>
        <small class="text-muted">39.90 €</small>
      </template>
    </b-card>

    <b-card title="Insecticide Cobra spécial rampants" img-src="https://picsum.photos/300/300/?image=41" img-alt="Image" img-top>
      <b-card-text>
        This card has supporting text below as a natural lead-in to additional content.
      </b-card-text>
      <template #footer>
        <small class="text-muted">19.90 €</small>
      </template>
    </b-card>

    <b-card title="Insecticide Cobra spécial volants" img-src="https://picsum.photos/300/300/?image=41" img-alt="Image" img-top>
      <b-card-text>
        This is a wider card with supporting text below as a natural lead-in to additional content.
        This card has even longer content than the first to show that equal height action.
      </b-card-text>
      <template #footer>
        <small class="text-muted">19.90 €</small>
      </template>
    </b-card>
  </b-card-group>
       </b-container>
   </div>
</template>

<script>
export default {
        data(){
        return {
            infoSection: {
            nomSection: "Produits",
            description: "Une gamme de produit diverse et variée."
        }
        }
    }

}
</script>

<style>

</style>