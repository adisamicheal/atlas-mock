<template>
  <div id="app">
    <Navbar class="navbar"/>
    <router-view/>
    <Footer />
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue"
import Footer from "./components/Footer.vue"
export default {
  components: {
    Navbar,
    Footer
  }
}
</script>

<style>
body{
  margin: 0;
  box-sizing: border-box;
}
#app{
  max-width: 1440px;
  position: relative;
  margin: auto;
}
.navbar{
  position: absolute;
  background: transparent;
  width: 100%;
}
.router-link-exact-active{
  border-bottom: 4px solid white;
}
@font-face {
  font-family: 'Xtreem Fat';
  src: url("assets/fonts/xtreem/XtreemFat_PERSONAL_USE.ttf");
}
@font-face {
  font-family: 'Xtreem Medium';
  src: url("assets/fonts/xtreem/XtreemMedium_PERSONAL_USE.ttf");
}
@font-face {
  font-family: 'Xtreem Thin';
  src: url("assets/fonts/xtreem/XtreemThin_PERSONAL_USE.ttf");
}
</style>
