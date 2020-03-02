<template>
  <div>
     <nav class="nav">
       <div class="nav-content">
         <div>
            <img src="../assets/icon/atlas.svg">
            <p>Atlas</p>
         </div>
         <div class="links">
           <ul>
             <li><router-link to="/" class="link">home</router-link></li>
             <li><router-link to="/features" class="link">features</router-link></li>
             <li><router-link to="/gallery" class="link">gallery</router-link></li>
             <li><router-link to="/contact" class="link">contact</router-link></li>
             <li><router-link to="/about" class="link">about</router-link></li>     
           </ul>
         </div>
       </div>
     </nav>

     <nav class="mobile-nav">
       <div class="mobile-nav-content">
         <div>
           <img src="../assets/icon/atlas.svg">
           <p>Atlas</p>
         </div>
         <div>
           <button class="navbar__button__mobile"  :class="{'open' : isOpen}" @click="isOpen = !isOpen">
            <span></span>
            <span></span>
            <span></span>
          </button>
         </div>
       </div>
      <div class="nav__mobile" :class="{'open' : isOpen}">
        <ul class="m-0 list-unstyled nav__mobile__list">
          <li class="nav__mobile__list__item" @click="isOpen = !isOpen">
            <router-link class="nav__mobile__link" to="/">Home</router-link>
          </li>
          <li class="nav__mobile__list__item" @click="isOpen = !isOpen">
            <router-link class="nav__mobile__link" to="/features">Features</router-link>
          </li>
          <li class="nav__mobile__list__item" @click="isOpen = !isOpen">
            <router-link class="nav__mobile__link" to="/gallery">Gallery</router-link>
          </li>
          <li class="nav__mobile__list__item" @click="isOpen = !isOpen">
            <router-link class="nav__mobile__link" to="/contact">Contact</router-link>
          </li>
          <li class="nav__mobile__list__item" @click="isOpen = !isOpen">
            <router-link class="nav__mobile__link" to="/about">About</router-link>
          </li>
        </ul>
      </div>
     </nav>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  data: () => ({
    isOpen: false,
  }),
};
</script>

<style scoped>
.nav-content{
  display: flex;
  justify-content: space-between;
  padding: 30px 60px;
}
.mobile-nav{
  display: none;
}
.nav__mobile {
  display: block;
  opacity: 0;
  max-height: 0px;
  background: #ffffff;
  z-index: 9000;
  transition: all .5s ease-in-out;
  padding: 2em 0;
  box-shadow: 0px 18px 20px rgba(0,0,0,0.2);
  position: absolute;
  top: 6em;
  width: 90vw;
  overflow: hidden;
}
.nav__mobile.open {
  opacity: 1;
  max-height: 70vh;
}
p{
  margin: 0;
  font-family: 'Roboto', sans-serif;
  font-size: 18px;
  color: white;
}
.links>ul{
  display: flex;
}
.link{
  text-decoration: none;
  color: white;
}
.link::after {
    content: '';
    display: block;
    width: 0;
    height: 4px;
    background: white;
    transition: width .3s;
}
:hover::after {
    width: 100%;
}
li{
  text-transform: uppercase;
  list-style: none;
  font-family: 'Roboto', sans-serif;
  font-size: 16px;
  line-height: 19px;
  /* color: #FFFFFF; */
  margin-right: 30px;
}
@media screen and (max-width: 768px){
  .nav-content{
    display: none;
  }
  .mobile-nav{
    display: block;
    padding: 20px 20px;
  }
  .mobile-nav-content{
    display: flex;
    justify-content: space-between;
  }
  .navbar__button__mobile {
  display: block;
  width: 48px;
  height: 40px;
  position: relative;
  transform: rotate(0deg);
  transition: .5s ease-in-out;
  cursor: pointer;
  background: transparent;
  border: none;
  }
  .navbar__button:focus,
  .navbar__button__mobile:focus {
    outline: 0;
  }
  .navbar__button__mobile > span {
    display: block;
    position: absolute;
    height: 6px;
    width: 100%;
    background: white;
    border-radius: 9px;
    opacity: 1;
    left: 0;
    transform: rotate(0deg);
    transition: .25s ease-in-out;
  }
  .navbar__button__mobile > span:nth-child(1) {
    top: 0px;
    transform-origin: left center;
  }

  .navbar__button__mobile > span:nth-child(2) {
    top: 15px;
    transform-origin: left center;
  }

  .navbar__button__mobile > span:nth-child(3) {
    top: 30px;
    transform-origin: left center;
  }

  .navbar__button__mobile.open > span:nth-child(1) {
    transform: rotate(45deg);
    top: -3px;
    left: 10px;
  }

  .navbar__button__mobile.open > span:nth-child(2) {
    width: 0%;
    opacity: 0;
  }

  .navbar__button__mobile.open > span:nth-child(3) {
    transform: rotate(-45deg);
    top: 30px;
    left: 10px;
  }
  .nav__mobile__list__item{
    padding: 1.5em 0;
  }
  .nav__mobile__link{
    color: black;
  }
}
</style>