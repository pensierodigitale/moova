<template>
  <div id="app">

     <transition name="slide-fade">
       <div v-if="showpanelmenu" class="slidepanel-menu">
<a class="navbar-item freccia" @click="showpanelmenu = !showpanelmenu"><span class="ion-android-arrow-forward"></span></a>
      <router-link to="/"><a class="navbar-item navlink-side" @click="showpanelmenu = !showpanelmenu">Home</a></router-link>
    <router-link to="/about"><a class="navbar-item navlink-side" @click="showpanelmenu = !showpanelmenu">About</a></router-link>
    <router-link to="/slide"><a class="navbar-item navlink-side" @click="showpanelmenu = !showpanelmenu">Slide</a></router-link>

        </div>

  </transition>
    <header class="navbar is-black">
        <div class="container">
        <div class="navbar-brand">
          <a class="navbar-item">
            <img src="http://res.cloudinary.com/thinkdigital/image/upload/v1508245585/logo-header_yqpxw0.png" alt="Logo">
          </a>

          <span class="navbar-burger burger" @click="showpanelmenu = !showpanelmenu">
            <span></span>
            <span></span>
            <span></span>
          </span>
        </div>
        <div id="navbarMenuHeroC" class="navbar-menu">
          <div class="navbar-end">
        <router-link to="/"><a class="navbar-item navlink">Home</a></router-link>
    <router-link to="/about"><a class="navbar-item navlink">About</a></router-link>
    <router-link to="/slide"><a class="navbar-item navlink">Slide</a></router-link>
          </div>
        </div>
      </div>
    </header>
    <!-- <img src="./assets/logo.png"> -->
   <transition name="page" mode="out-in">
    <router-view></router-view>
    </transition>
  </div>
</template>

<script>

export default {
  name: 'app',
  data () {
    return {
      isImageModalActive: false,
      isCardModalActive: false,
      isMenuModalActive: false,
      showpanel: false,
      show: false,
      showpanelmenu: false,
      checkedNames: []
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 0px;
  background-color: #000;
}

.page-enter-active, .page-leave-active {
  transition: opacity 1.5s, transform 1.5s;
}
.page-enter, .page-leave-to {
  opacity: 0;
  transform: translateY(20px);
  /*transform: translate(100px);*/
 

}

.navlink{
  font-weight: bold;
  font-size: 22px;
  color: #fff;
}

.freccia {
    font-weight: bold;
    font-size: 22px;
    color: #fff;
    position: relative;
    font-size: 33px;
    float: right;
    right: 12px;
}
.navlink-side{
  position: relative;
  top: 100px;
  font-weight: bold;
  font-size: 22px;
  color: #fff;
}
.slide-fade-enter-active {
    transition: all .3s ease;
}

.slide-fade-leave-active {
    transition: all .3s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}

.slide-fade-enter,
.slide-fade-leave-to
/* .slide-fade-leave-active below version 2.1.8 */

{
    transform: translateX(100%);
    opacity: 1;
}

.slide-fade-panel-enter-active {
    transition: all .3s ease;
}

.slide-fade-panel-leave-active {
    transition: all .8s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}

.slide-fade-panel-enter,
.slide-fade-panel-leave-to {
    transform: translateX(-100%);
    opacity: 1;
}

.slidepanel {
    position: fixed;
    background: #ddd;
    width: 300px;
    height: 100vh;
    right: 0px;
    top: 0px;
    bottom: 0px;
    z-index: 9;
}

.slidepanel-menu {
    position: fixed;
    background: #121212;
    width: 300px;
    height: 100vh;
    right: 0px;
    top: 0px;
    bottom: 0px;
    z-index: 9;
}

.slidepanel-left {
    position: fixed;
    background: #ddd;
    width: 49%;
    height: 100vh;
    left: 0px;
    top: 0px;
    bottom: 0px;
    z-index: 9;
}

/*.navbar-burger.is-active span:first-child {
    margin-left: -5px;
    -webkit-transform: rotate(45deg);
    transform: rotate(45deg);
    -webkit-transform-origin: left top;
    transform-origin: left top;
    color: #fff;
}

.navbar-burger.is-active span:nth-child(2) {
    opacity: 0;
    color: #fff;
}

.navbar-burger.is-active span:nth-child(3) {
    margin-left: -5px;
    -webkit-transform: rotate(-45deg);
    transform: rotate(-45deg);
    -webkit-transform-origin: left bottom;
    transform-origin: left bottom;
    color: #fff;
}*/


.cover {

    background-size: cover;
    background-position: top;
    position: relative;
    width: 100%;
}
</style>
