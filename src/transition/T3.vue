<template>
    <transition @leave="animate" @enter="animate" name="t3" mode="out-in">
        <slot></slot>
    </transition>
</template>
<script>
import ShapeOverlay from '@/transition/T3Class';
export default {
  name: 'T3',
  mounted: function () {
    const shC = document.querySelector('#shape-container');
    shC.classList.add('demo-3');
    const html = '<path class="shape-overlays__path"></path><path class="shape-overlays__path"></path><path class="shape-overlays__path"></path>';
        const shO = document.querySelector('.shape-overlays');
        shO.innerHTML = html;
        this.shapeOverlays = new ShapeOverlay(shO);
    },
    beforeDestroy: function () {
        this.shapeOverlays = null;
    },
    methods: {
        animate(el, done) {
        this.shapeOverlays.toggle(done);
    }
  }
}
</script>

<style>
.t3-enter-active, .t3-leave-active {
  transition: opacity 2s;
}
.t3-enter, .t3-leave-to {
  opacity: 0;
}
</style>
