<template>
    <main>
       <div class="footer-content">
           <div class="footer-up">
                <div class="footer-up-content">
                    <ul class="blue-link">
                        <li  v-for = "(element, index) in blueBar" :key = "index">
                            <img :src="element.img" alt="">
                            <a class="nav-link active"  href="#">{{element.name}}</a>
                        </li>
                    </ul>
              </div>
           </div>
           <div class="footer-central">
               <div class="footer-ul">
                    <ul>
                        <li class="title">dc comics</li>
                        <li> <a href="">Characters</a></li>
                        <li> <a href="">Comics</a></li>
                        <li> <a href="">Movie</a></li>
                        <li><a href="">TV</a></li>
                        <li><a href="">Games</a></li>
                        <li><a href="">Videos</a></li>
                        <li><a href="">News</a></li>
                    </ul>
                    <ul>
                        <li class="title">dc</li>
                        <li> <a href="">Terms Of Use</a></li>
                        <li> <a href="">Privacy Policy(New)</a></li>
                        <li> <a href="">Advertising</a></li>
                        <li><a href="">Jobs</a></li>
                        <li><a href="">Subscriptions</a></li>
                        <li><a href="">CPSC Certificates</a></li>
                        <li><a href="">Ratings</a></li>
                        <li><a href="">Shop Help</a></li>
                        <li><a href="">Contact Us</a></li>
                    </ul>
                    <ul>
                        <li class="title">sites</li>
                        <li> <a href="">DC</a></li>
                        <li> <a href="">DC UNIVERSE INFINITE</a></li>
                        <li> <a href="">DC Kids</a></li>
                        <li><a href="">DC Shop</a></li>
                        <li><a href="">Subscriptions</a></li>
                        <li><a href="">MAD Magazine</a></li>
                    </ul>
                    <ul>
                        <li class="title">dc Shop</li>
                        <li> <a href="">Shop Dc</a></li>
                        <li> <a href="">Shop DC collectibles</a></li>
                    </ul>
                    <p>All Site Content TM and © 2020 DC Entertainment, unless otherwise <a href="">noted here</a>. All rights reserved.</p>
                    <p><a href="">Cookies Settings</a></p> 
               </div> 
               <div class="background-logo"></div>
           </div>
           <div class="footer-bottom">
               <div class="bottom-left">
                   <button type="button" class="btn btn-outline-primary">SIGN-UP NOW!</button>
               </div>
               <div class="bottom-right">
                   <h3>Follow us</h3>
                   <div class="social">
                       <img src="https://www.dccomics.com/sites/all/themes/dc_comics_bp/images/footer-facebook.png" alt="">
                       <img src="https://www.dccomics.com/sites/all/themes/dc_comics_bp/images/footer-twitter.png" alt="">
                       <img src="https://www.dccomics.com/sites/all/themes/dc_comics_bp/images/footer-youtube.png" alt="">
                       <img src="https://www.dccomics.com/sites/all/themes/dc_comics_bp/images/footer-pinterest.png" alt="">
                       <img src="https://www.dccomics.com/sites/all/themes/dc_comics_bp/images/footer-periscope.png" alt="">
                   </div>
               </div>
           </div>
       </div>
    </main>
</template>

<script>

export default{
    name: 'Footer',
    props:[
        'blueBar'
        ]
    
}
        
</script>
<style scoped lang="sass">
 .footer-up
    background-color: #0282F9

    .footer-up-content
        padding: 30px 0

        .blue-link
            width: 100%
            display: inline-flex
            justify-content: space-around
            align-items: center
            margin: 10px 0

            li
                display: inline-flex
                align-items: center
                justify-content: center
                align-content: center

                img
                    max-height: 50px

                a
                    color: white
                    text-transform: uppercase
.footer-central
    padding: 60px 150px
    background: #3d3d3d
    display: flex
    

    .footer-ul
        display: inline-flex
        width: 45%
        flex-wrap: wrap
        ul
            padding: 0
            padding-right: 35px
        
        .title
            color: white
            text-transform: uppercase
            font-size: 20px
            font-weight: 700
        li
            a
                color: #a0a0a0
                font-size: 12px
                text-decoration: none
                &:hover
                    color: #0282F9
        p
            color: #a0a0a0
            font-size: 12px
            a
                text-decoration: none
    .background-logo
        background-image: url('https://www.dccomics.com/sites/all/themes/dc_comics_bp/images/logo-background-v2.png')
        width: 65%
        background-position: center
        background-repeat: no-repeat
.footer-bottom
    background: #4f4f4f
    width: 100%
    display: inline-flex
    align-content: center
    justify-content: space-between
    align-items: center
    padding: 30px 100px
    .btn
        border-radius: 0
    .bottom-right
        display: inline-flex
        align-items: center
        align-content: center
        h3
            padding-right: 30px
            color:#0282F9
            text-transform: uppercase
        .social
            img
                margin-right: 10px

</style>
