<template>
 <section>
  
<agile>
            <div class="slide">
                <h3>slide 1</h3>
            </div>
            <div class="slide">
                <h3>slide 2</h3>
            </div>
        </agile>

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
import Vue from 'vue'
import VueAgile from 'vue-agile'
Vue.use(VueAgile)
export default {
  name: 'Slide'
}
</script>

<style>
.agile__dot button {
    background-color: #eee;
    border: none;
    border-radius: 50%;
    cursor: pointer;
    display: block;
    height: 15px !important;
    font-size: 0;
    line-height: 0;
    margin: 0;
    -webkit-transition-duration: .3s;
    transition-duration: .3s;
    width: 15px !important;
    margin-bottom: 9px !important;
}

.agile__arrow {
    border: none;
    bottom: 10px;
    margin: 0;
    padding: 0;
    position: absolute;
    -webkit-transition-duration: .3s;
    transition-duration: .3s;
    color: #fff !important;
}

.agile__arrow svg{
   
    fill:  transparent !important;
}
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