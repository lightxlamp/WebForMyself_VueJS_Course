<template>
    <div>
      <h4>Car: {{ $route.query.car}}</h4>
      <h5>Car year: {{ year }}</h5>

      <div class="scroll"></div>
      <h6 id="scroll">Hello from the bottom</h6>
      <div class="scroll"></div>
    </div>
</template>

<script>
    export default {
      computed: {
        year(){
          return this.$route.query.year
        }
      }
      // ,
      // beforeRouteEnter(to, fromR, next){
      //   console.log('beforeRouteEnter')
      // }
    }
</script>

<style scoped>
  .scroll{
    width: 100px;
    height: 1000px;
    background-color: #cccccc;
  }
</style>
