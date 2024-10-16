<template>
  <div id="app">
    <nav> 
       <AppHeader/>
    </nav>
  
    <router-view/>
  </div>
</template>
<script>
import AppHeader from './components/AppHeader.vue';
export default{
  components:{
    AppHeader
  },
}
</script>


<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #253241;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #cbd1d8;

    &.router-link-exact-active {
      color: #25c760;
    }
  }
}
</style>
