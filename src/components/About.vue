<template>
 <section>
 	

  <!-- Hero head: will stick at the top -->
      <!-- navigation -->
   <!--      <header class="navbar is-black">
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
    <div class="hero is-primary is-large" id="intro" style="background-image: url(http://res.cloudinary.com/thinkdigital/image/upload/v1509475974/gradeint-5_vhfbk1.jpg);">
  <!-- Hero content: will be in the middle -->
  <div class="hero-body">
    <div class="container has-text-left">
      <h1 class="title intro-title">
         Become an #AngelBiker!
      </h1>
      <h2 class="subtitle intro-sub-title has-text-left">
       enjoy the bike revolution.
      </h2>
    </div>
  </div>

  <!-- Hero footer: will stick at the bottom -->
</div>
    <transition name="slide-fade">
       <div v-if="showpanelmenu" class="slidepanelmenu">
<a @click="showpanelmenu = !showpanelmenu">ssss</a>
<nuxt-link class="navbar-item" to="/">Home</nuxt-link>
    <nuxt-link class="navbar-item" to="/one">One</nuxt-link>
    <nuxt-link class="navbar-item" to="/About">About</nuxt-link>
        </div>

  </transition>

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
<!-- 
    <no-ssr placeholder="Loading...">
    <agile :arrows="true" :speed="750"
    :timing="'linear'" :fade="false"
    :autoplay="false" :pauseOnHover="false" >
          <div class="slide slide--1"><h3>slide 1</h3></div>
    <div class="slide slide--2"><h3>slide 2</h3></div>
    <div class="slide slide--3"><h3>slide 3</h3></div>
    <div class="slide slide--4"><h3>slide 4</h3></div>
    <div class="slide slide--5"><h3>slide 5</h3></div>
    <div class="slide slide--6">
        <div class="block">
   <div class="columns columns is-desktop is-vcentered">
  <div class="column ">

 <h1 class="title has-text-centered ">
        Primary bold title
      </h1>
      <h2 class="subtitle has-text-centered">
        Primary bold subtitle
      </h2>
  </div>
  <div class="column">
     <figure class="image  is-centered">
  <img src="http://res.cloudinary.com/thinkdigital/image/upload/v1498985700/banner_contact_building_cvedmz.png"/>
</figure>
  </div>

</div>
</div>

    </div>
    </agile>
</no-ssr>
 -->
<!-- 
    <div class="hero-body">
    <div class="container">
     <figure class="image is-2by1">
  <img src="https://www.satispay.com/app/themes/roots/assets/img/header_home.svg"/>
</figure>
      
       <h1 class="title has-text-centered">
        Primary bold title
      </h1>
      <h2 class="subtitle has-text-centered">
        Primary bold subtitle
      </h2>
    </div>
  </div> -->
     


        <div class="block ">
            <div class="columns columns is-desktop is-vcentered">
    
                <div class="column cover">
                  <figure class="image  is-centered">
  <img src="http://via.placeholder.com/450x400"/>
</figure>
                </div>
                            <div class="column ">
                    <h1 class="title has-text-centered ">
        Primary bold title
      </h1>
                    <h2 class="subtitle has-text-centered">
        Primary bold subtitle
      </h2>
                </div>
            </div>
        </div>

    <div class="hero-foot">
      <div class="container">
        <div class="tabs is-centered">
          <ul>
            <li><a>And this at the bottom</a></li>
          </ul>
        </div>
      </div>
</div>

<footer class="footer is-primary is-bold">
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
  name: 'About'
}
</script>

<style>

.intro-title{
  font-weight: 900;
  font-size: 5rem;
}

.intro-sub-title{
  font-weight: 600;
  font-size: 2rem;
}
.purple {
    background-color: purple;
    height: 50px;
  width: 50px;
    margin: 10px;
}

.darkgreen {
    background-color: darkgreen;
    height: 50px;
  width: 50px;
    margin: 10px;
}

.darkred {
    background-color: darkred;
    height: 50px;
  width: 50px;
    margin: 10px;
}
#intro {
    
    background-size: cover;
    background-position: center center;
    position: relative;
}
/*.page-enter-active, .page-leave-active {
  transition: all .45s ease-out;
}
.page-enter, .page-leave-active {
  opacity: 0;
  transform-origin: 50% 50%;

}*/

/* scale and fade */

.pt-page-scaleDown {
  animation: scaleDown .7s ease both;
}

.pt-page-scaleUp {
  animation: scaleUp .7s ease both;
}

.pt-page-scaleUpDown {
  animation: scaleUpDown .5s ease both;
}

.pt-page-scaleDownUp {
  animation: scaleDownUp .5s ease both;
}

.pt-page-scaleDownCenter {
  animation: scaleDownCenter .4s ease-in both;
}

.pt-page-scaleUpCenter {
  animation: scaleUpCenter .4s ease-out both;
}

/************ keyframes ************/

/* scale and fade */

@keyframes scaleDown {
  to { opacity: 0; transform: scale(.8); }
}

@keyframes scaleUp {
  from { opacity: 0; transform: scale(.8); }
}

@keyframes scaleUpDown {
  from { opacity: 0; transform: scale(1.2); }
}

@keyframes scaleDownUp {
  to { opacity: 0; transform: scale(1.2); }
}

@keyframes scaleDownCenter {
  to { opacity: 0; transform: scale(.7); }
}

@keyframes scaleUpCenter {
  from { opacity: 0; transform: scale(.7); }
}
.slide {
    color: #fff;
    height: 650px;
    position: relative;
    background-color: #f1c40f;

    }

   

    h3 {
        font-size: 32px;
        font-weight: 300;
        left: 50%;
        margin: 0;
        position: absolute;
        top: 50%;
        transform: translate(-50%, -50%);
    }



    .agile__dots {
        bottom: 0;
        left: 50%;
        position: absolute;
        transform: translateX(-50%);
}

.agile__dot {
    margin: 0 10px;
}

.agile__dot__current {
    
    width: 2px;
    height: 2px;
    color:#60439a;
}

.agile__dot button {
    background-color: transparent;
    border: 1px solid #fff;
}
.agile__dot button {
    background-color: #eee;
    border: none;
    border-radius: 50%;
    cursor: pointer;
    display: block;
    height: 10px;
    font-size: 0;
    line-height: 0;
    margin: 0;
    transition-duration: .3s;
    width: 10px;
}
            .agile__dot button:hover {
                background-color: #fff;
            }

             .agile__dot__current button {
                background-color: #fff;
            }
            button, button {
    background-color: transparent;
    border: none;
    cursor: pointer;
    padding: 0;
}

 .agile__arrow {
    width: 80px;
}
.agile__arrow {
    height: 100%;
    top: 0;
    width: 50px;
}
.agile__arrow--prev {
    left: 0;
}
.agile__arrow {
    border: none;
    bottom: 10px;
    margin: 0;
    padding: 0;
    position: absolute;
    transition-duration: .3s;
}
.agile__arrow--next {
    right: 0;
}
#prova{
  position: relative;
  opacity:
}

</style>	