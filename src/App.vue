<template>
  <div class="app" >
    <NavBar/>
   <router-view />
</div>
</template>

<script>
import NavBar from './components/NavBar.vue';

export default {
  name: 'App',
  components: {
    NavBar
  }
};
</script>

<style>
.app {
  font-family: 'Courier New', Courier, monospace;
  max-width: 100%;
  text-align: center;
  align-items: center;
  color: black;
  width:100%;
  height:100vh;
  background-color: white;
}

</style>
