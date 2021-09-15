<template>
  <div id="app">
    
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import ComicJson from './json/dc-comics.json'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
  },
  data: function(){
    return{
      comics: ComicJson,

    }
  },
  created(){
    console.log(this.comics);

  },
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
