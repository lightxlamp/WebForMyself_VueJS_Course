<template>
  <h2>Counter #2 {{counter}}</h2>
</template>

<script>
  export default{
    computed: {
      counter () {
        return this.$store.getters.computedCounter
      }
    }
  }
</script>

