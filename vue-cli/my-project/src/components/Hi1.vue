<template>
  <div>
      <p>{{hi}}-{{$route.params.name}}-{{$route.params.id}}</p>
  </div>
</template>

<script>
export default {
  name: 'Hi1',
  data () {
    return {
      hi: '我是Hi1页面'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
