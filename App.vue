<template>
  <v-app>

    <v-content>
      <AppBar/>
      <HelloWorld/>
      <MainPage/>
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';
import AppBar from './components/AppBar';
import MainPage
export default {
  name: 'App',

  components: {
    HelloWorld,
    AppBar,

  },

  data: () => ({
    
  }),
};
</script>
