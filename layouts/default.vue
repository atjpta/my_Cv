<template>
  <div>
    <OtherVDialog />
    <OtherVHeader />
    <OtherVAlert />

    <slot />
    <OtherBottom />
  </div>
</template>

<script setup>

</script>

<style>
.router-link-exact-active {
  color: rgb(255, 255, 255);
  background: rgba(120, 0, 255);
}
.bounce-enter-active {
  animation: bounce-in 0.5s;
}
.bounce2-leave-active {
  animation: bounce-in 0.5s reverse;
}
@keyframes bounce-in {
  0% {
    transform: scale(0);
  }
  100% {
    transform: scale(1);
  }
}
</style>
