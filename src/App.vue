<template>
  <div id="app">
    <WelcomeMessage :msg="msg"/>
    
  </div>
</template>

<script>
  import WelcomeMessage from './components/WelcomeMessage'

  export default {
    name: 'App',
    data(){
      return{
        msg: 'Welcome, here'
      }
    },
    components: {
      WelcomeMessage,
    }
  }
</script>

<style>

</style>
