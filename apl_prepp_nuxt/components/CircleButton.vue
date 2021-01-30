<template>
  <div>
    <div class="rounded-full h-24 w-24 flex items-center justify-center bg-red-500" />
    <h3>{{ universitys.chalmers }}</h3>
  </div>
</template>

<script>
export default {
  name: 'CircleButton',
  data () {
    return {
      universitys: {
        chalmers: 'Chalmers',
        gbgUnity: 'Göteborgs Universitet'
      }
    }
  }
  // props: ['icon', 'schoolname'],
}
</script>
