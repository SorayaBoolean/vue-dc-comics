<template>
  <div id="app">
    <MyHeader/>
    <MyMain/>
    <MyFooter/>
    
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import MyMain from './components/MyMain.vue';
import MyFooter from './components/MyFooter.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter
}
}
</script>

<style lang="scss">

@import './styles/general.scss';
@import './styles/vars.scss';

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
ul {
  list-style-type: none;
  padding: 0;

  li a{
    text-decoration: none;
    color: black;
  }
}
</style>
