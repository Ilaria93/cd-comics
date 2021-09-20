<template>
 <main>
   <div class="navbar-up"></div>
   <!-- Navbar content -->
  <div class="container-fluid">
    <div class="row">
      <div class="col-12">
        <div class="navbar-down">
          <nav class="navbar navbar-expand-lg navbar-light bg-light">
            <div class="navbar-content">
              <div class="image-content">
                <img src="../assets/dc-logo.png" alt="">
              </div>
              <div class="navlist-content">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                  <li  v-for = "element in navList" :key = "element.id" class="nav-item">
                    <a class="nav-link active"  href="element.link">{{element.name}}</a>
                  </li>
                </ul>
              </div>
              <div class="serach-content">
                <form class="d-flex">
                  <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
                  <button class="btn btn-outline-success" type="submit">Search</button>
                </form>
              </div>
            </div>
          </nav>
        </div>
      </div>
    </div>
  </div>
 </main>
</template>

<script>
export default {
  name: 'Header',
  props:[
        'navList'
        ]
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="sass">

.navbar-up
  background-color: #0282F9
  height: 40px
  width: 100%
.navbar-content
  display: inline-flex
  width: 100%
  align-items: center
  justify-content: space-around
  padding: 15px
.image-content
  width: 80px
  height: 80px
  img
    width: 100%

.navlist-content
  a
    text-transform: uppercase
    font-size: 18px
    font-weight: bold
    &:hover
      color: #0282F9 !important
</style>
