<template>
  <div class="h-screen">
    <Navbar />
    <div class="absolute flex flex-col place-self-center w-4/5 m-auto" id="canvas">
      <div class="flex justify-between ">
        <CircleButton />
        <CircleButton />
        <CircleButton />
        <CircleButton />
        <CircleButton />
      </div>
      <div class="flex justify-between w-2/6 m-auto">
        <NavigationButton />
        <NavigationButton />
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from '../components/Navbar.vue'
import CircleButton from '../components/CircleButton.vue'
import NavigationButton from '../components/NavigationButton.vue'

export default {
  name: 'Welcome',

  components: {
    Navbar,
    CircleButton,
    NavigationButton
  }
}
</script>

<style>
#canvas {
  top: 50%; right: 50%;
  transform: translate(50%,-50%);
  height: 300px;
}
</style>
