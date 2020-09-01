<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
const { remote } = window.require('electron')
export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  mounted () {
    console.log('remote', remote)
  }
}
</script>
