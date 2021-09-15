<template>
    <main>
        <div class="container">
            <div class="row">
                <Card v-for="(element, index) in comics" :key="index" 
                :thumb="element.thumb"
                :price="element.price"
                :type="element.type"
                :title="element.series"/>
            </div>
        </div>
    </main>
</template>

<script>
import Card from './Card.vue'

export default{
    name: 'Main',
    components:{
        Card,
    },
    props:{
        comics: Array
    },
    cerated(){
        console.log(this.comics);
    }
}
        
</script>
<style scoped lang="sass">
main
    background-color:  black
    color: white


</style>
