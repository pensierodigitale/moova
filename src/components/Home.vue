<template>
  
   <section>
      <!-- Hero head: will stick at the top -->



    <!-- navigation -->
    <!--     <header class="navbar is-black">
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
    <nuxt-link class="navbar-item" to="/">Home</nuxt-link>
    <nuxt-link class="navbar-item" to="/one">One</nuxt-link>
    <nuxt-link class="navbar-item" to="/About">About</nuxt-link>
            <span class="navbar-item">
              <a class="button is-success is-inverted">
               
                <span>Contact</span>
              </a>
            </span>
          </div>
        </div>
      </div>
    </header> -->
    <div class="hero is-primary is-large" id="intro" style="background-image: url(http://res.cloudinary.com/thinkdigital/image/upload/v1509534517/gr-2_lljoxx.jpg);">
  <!-- Hero content: will be in the middle -->
  <div class="hero-body">
<div class="container">
    <div class="tile is-ancestor">
      <div class="tile is-parent is-6 is-vertical">
        <div class="tile is-child">
          <h1 class="title push-down-2 intro-title-one ">Lifecycle Social Advertising.</h1>
          <b class="subtitle intro-sub-title-one">Technology to help you acquire more leads, reduce cost per lead and increase downstream conversion.</b>
        </div>
      </div>
    </div>
  </div>
  </div>

  <!-- Hero footer: will stick at the bottom -->
</div>
  <!-- Hero content: will be in the middle -->
 

    <div class="hero is-medium is-warning is-bold">    
      <div class="hero-body">
        <div class="container">
          <p class="title">
            Warning bold title
          </p>
          <p class="subtitle">
            Warning bold subtitle
          </p>
        </div>
      </div>
    </div>
    
        <div class="block ">
            <div class="columns columns is-desktop is-vcentered">
                <div class="column ">
                    <h1 class="title has-text-centered ">
        Primary bold title
      </h1>
                    <h2 class="subtitle has-text-centered">
        Primary bold subtitle
      </h2>
                </div>
                <div class="column cover">
                  <figure class="image  is-centered">
  <img src="http://via.placeholder.com/450x400"/>
</figure>
                </div>
            </div>
        </div>
 <!--    <div class="hero-foot">
      <div class="container">
        <div class="tabs is-fullwidth">
  <ul>
    <li>
      <a>
        <span class="icon"><i class="fa fa-angle-left"></i></span>
        <span>Left</span>
      </a>
    </li>
    <li>
      <a>
        <span class="icon"><i class="fa fa-angle-up"></i></span>
        <span>Up</span>
      </a>
    </li>
    <li>
      <a>
        <span>Right</span>
        <span class="icon"><i class="fa fa-angle-right"></i></span>
      </a>
    </li>
  </ul>
</div>
      </div>
</div> -->



<footer class="footer">
  <div class="container">
    <div class="content has-text-centered">
      <p>
        <strong>Bulma</strong> by <a href="http://jgthms.com">Jeremy Thomas</a>. The source code is licensed
        <a href="http://opensource.org/licenses/mit-license.php">MIT</a>. The website content
        is licensed <a href="http://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY NC SA 4.0</a>.
      </p>
    </div>
  </div>
</footer>

    
    </section>
 
</template>

<script>
  export default {
    name: 'Home',
    data () {
      return {
        msg: 'Welcome to Crypto Info'
      }
    }
  }
</script>

<style>
#intro {
    
    background-size: cover;
    background-position: center center;
    position: relative;
}

.drop-color-bg-verde{
  background-color: #115742;
}

.drop-color-verde{
  color: #115742;
}

.drop-color-bg-blu{
  background-color: #072186;
}

.drop-color-blu{
  color: #072186;
}
.drop-color-bg-rosa{
  background-color: #fcb0a0;
}

.drop-color-rosa{
  color: #fcb0a0;
}

.drop-color-bg-giallo{
  background-color: #fdcc8d;
}

.drop-color-giallo{
  color: #fdcc8d;
}

.intro-title-one{
  font-weight: 900;
  font-size: 3.5rem;
}

.intro-sub-title-one{
  font-weight: 600;
  font-size: 1.5rem;
}

.fadeOpacity-enter-active, .fadeOpacity-leave-active {
  transition: opacity .35s ease-out;
}

.fadeOpacity-enter, .fadeOpacity-leave-active {
  opacity: 0;
  background-color:#eb553c;
}
.homepage-hero {
    background-image: url(http://res.cloudinary.com/thinkdigital/image/upload/v1508496127/Header_zw2uno.png);
    background-size: cover;
    background-position: top;
    min-height: 620px;
    position: relative;
}

a.navbar-item:hover{
background-color:transparent !important;
opacity: 0.8;
  
}

.button.is-success.is-inverted.is-outlined {
    background-color: transparent;
    border-color: #fff;
    color: #fff;
    margin:5px;
}
.hero .navbar {
    background: #0a0a0a;
}
.hero .navbar .is-black {
    background-color: #0a0a0a;
}


a.navbar-item .modal-menu:hover {
    background-color: transparent !important;
    opacity: .8;
}
a.navbar-item .modal-menu {
    fonnt-size:33px;
}

a.navbar-item.modal-menu{
    background-color: transparent;
    color: #fff;
    font-size:33px;
    line-height:30px;
}
a.navbar-item.modal-menu:hover {
   background-color: transparent;
    color: #ccc;
    font-size:33px;
    line-height:30px;
}

.modal-close.is-large {
    height: 32px;
    max-height: 32px;
    max-width: 32px;
    min-height: 32px;
    min-width: 32px;
    width: 32px;
    position: absolute;
    top: 11px;
    right: 9px;
}

modal-card, .modal-content {
    margin: 0 auto;
    width: 900px;
}


</style>

