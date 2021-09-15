<template>
    <div class="product-card col-2 ">
        <div class="img-container px-15" :style= "{ backgroundImage: 'url(' + thumb + ')'}"></div>
        <h3>Titolo: {{title}}</h3>
        <h4>Prezzo: {{price}}</h4>
        <h4> Serie: {{type}}</h4>
    </div>
</template>

<script>


export default ({
    name: 'Card',
    props:{
        thumb: String,
        price: String,
        title: String,
        type: String
    }
})
</script>
<style scoped lang="sass">
    @import '../style/app'


</style>
