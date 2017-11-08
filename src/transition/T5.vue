<template>
    <transition @leave="animate" @enter="animate" name="t3" mode="out-in">
        <slot></slot>
    </transition>
</template>
<script>
import ShapeOverlay from '@/transition/T5Class';
export default {
  name: 'T5',
  mounted: function () {
    const shC = document.querySelector('#shape-container');
    shC.classList.add('demo-5');
    const html = '<path class="shape-overlays__path"></path><path class="shape-overlays__path"></path>';
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
.t5-enter-active, .t5-leave-active {
  transition: opacity 2s;
}
.t5-enter, .t5-leave-to {
  opacity: 0;
}
</style>
