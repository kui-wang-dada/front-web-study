<template>
  <div id="app">
    <a-layout class="layout">
      <a-layout-header><HeaderTop></HeaderTop></a-layout-header>

      <a-layout-content>
        <router-view></router-view>
      </a-layout-content>

      <a-layout-footer>Footer</a-layout-footer>
    </a-layout>
  </div>
</template>
<script>
import HeaderTop from '@/components/HeaderTop.vue';
export default {
  components: { HeaderTop }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100%;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
