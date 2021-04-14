<template>
  <div id="app">
    <WelcomeMessage :msg="msg"/>
    <show-hide :canSee="canSee"></show-hide>
    <button @click="handleChangeButton">{{ !canSee ? "Show":"Hide" }}</button>

  </div>
</template>

<script>
  import WelcomeMessage from './components/WelcomeMessage'
  import ShowHide from './components/ShowHide'

  export default {
    name: 'App',
    data(){
      return{
        msg: 'Welcome, here',
        canSee: false,
      }
    },
    methods:{
      handleChangeButton:()=>{
        console.log(this.canSee)
      }
    },
    components: {
      WelcomeMessage,
      ShowHide,
    }
  }
</script>

<style>

</style>
