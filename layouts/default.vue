<template>
  <div>
    <TheNavigation />
    <hr />
    <nuxt />
  </div>
</template>

<script>
import TheNavigation from '../components/Navigation/TheNavigation'
export default {
  components: { TheNavigation }
}
</script>

<style>
/* Page-transition styles must be global */

/* page is used by default */
.page-leave-active,
.page-enter-active {
  transition: opacity 0.3s;
}
.page-enter,
.page-leave-to {
  opacity: 0;
}

/* slide-right */
.slide-right-leave-active,
.slide-right-enter-active {
  transition: all 0.3s;
}
.slide-right-enter {
  opacity: 0;
  transform: translate(-30px, 0);
}
.slide-right-enter-to,
.slide-right-leave {
  opacity: 1;
  transform: translate(0, 0);
}
.slide-right-leave-to {
  opacity: 0;
  transform: translate(30px, 0);
}

/* slide-left */
.slide-left-leave-active,
.slide-left-enter-active {
  transition: all 0.3s;
}
.slide-left-enter {
  opacity: 0;
  transform: translate(30px, 0);
}
.slide-left-enter-to,
.slide-left-leave {
  opacity: 1;
  transform: translate(0, 0);
}
.slide-left-leave-to {
  opacity: 0;
  transform: translate(-30px, 0);
}

/* swipe-right */
.swipe-right-leave-active,
.swipe-right-enter-active {
  transition: all 0.3s;
}
.swipe-right-enter {
  opacity: 0;
  transform: translate(-100%, 0);
}
.swipe-right-enter-to,
.swipe-right-leave {
  opacity: 1;
  transform: translate(0, 0);
}
.swipe-right-leave-to {
  opacity: 0;
  transform: translate(100%, 0);
}

/* jump */
.jump-leave-active,
.jump-enter-active {
  transition: all 0.3s;
}
.jump-enter {
  opacity: 0;
  transform: rotate(-12deg);
}
.jump-enter-to,
.jump-leave {
  opacity: 1;
  transform: rotate(0deg);
}
.jump-leave-to {
  opacity: 0;
  transform: rotate(12deg);
}
</style>
