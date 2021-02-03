<template>
  <div>
    <button id ="universityBTN" class="rounded-full h-24 w-24 flex items-center justify-center border-4 border-light-blue-500 ">
      <h3>{{ universitys.chalmers }}</h3>
    </button>
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

<style>
#universityBTN:focus{
  border-color: rgba(248, 113, 113);
  background-color: rgba(254, 202, 202);
};

</style>
