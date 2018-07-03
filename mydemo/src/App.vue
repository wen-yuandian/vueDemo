<template>
  <div id="app">
    <tab></tab>
    <router-view/>
  </div>
</template>

<script>
import Tab from 'components/tab/tab'


export default {
  name: 'App',
  components: {
    Tab
  },
  methods:{
   
  }
}

</script>

<style lang="stylus">
* 
  margin 0
  padding 0

#app 
  font-family 'Avenir', Helvetica, Arial, sans-serif
  -webkit-font-smoothing antialiased
  -moz-osx-font-smoothing grayscale
  text-align center
  color #2c3e50
  margin-top 60px

pad(x,y)
		padding x y
</style>
