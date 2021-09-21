<template>
  <div id="app">
    
    <Header :navList ="nav"/>
    <Main :comics="comics"/>
    <Footer :blueBar ="footerBlue" />
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
      ],
      footerBlue:[
        {
        img:'https://www.dccomics.com/sites/all/themes/dc_comics_bp/images/buy-bar-DCUI.svg',
        name: 'Digital comics'
        },
        {
        img:'https://www.dccomics.com/sites/all/themes/dc_comics_bp/images/buy-bar-DCshop.svg',
        name: 'Dc merchandise'
        },
        {
        img: 'https://www.dccomics.com/sites/all/themes/dc_comics_bp/images/buy-bar-subscription.svg',
        name: 'Subscription'
        },
        {
        img: 'https://www.dccomics.com/sites/all/themes/dc_comics_bp/images/buy-bar-locator.svg',
        name: 'Comic shop locator'
        }
      ]

    }
  },
  
}
</script>

<style lang="sass">
    @import './style/app.sass'
</style>
