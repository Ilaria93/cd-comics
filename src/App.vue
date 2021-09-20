<template>
  <div id="app">
    
    <Header :navList ="nav"/>
    <Main :comics="comics"/>
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
      nav:[
        {
          id:0,
          name:'Characters',
          link: '/characters'
        },
        {
          id:1,
          name:'Comics',
          link: '/comics'
        },
        {
          id: 2,
          name: 'Movies',
          link: '/movies'
        },
        {
          id: 3,
          name: 'TV',
          link: '/tv'
        },
        {
          id: 4,
          name: 'Games',
          link: '/games'
        },
        {
          id: 5,
          name: 'Videos',
          link: '/videos'
        },
        {
          id: 6,
          name: 'News',
          link: '/news'
        },
        {
          id: 7,
          name: 'Shop',
          link: '/shop'
        }
      ]

    }
  },
  
}
</script>

<style lang="sass">
    @import './style/app.sass'
</style>
