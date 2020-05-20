<template>
  <v-app>

    <v-content>
      <!-- <AppBar/> -->
      <!-- <HelloWorld/> -->
      <!-- <MainPage/> -->
      <Tasks_AppBar/>
    </v-content>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld';
// import AppBar from './components/AppBar';
// import MainPage from './components/MainPage';
// import Tasks_main from './components/Tasks_main';
import Tasks_AppBar from './components/Tasks_AppBar';

export default {
  name: 'App',

  components: {
    // HelloWorld,
    // AppBar,
    // MainPage,
    // Tasks_main,
    Tasks_AppBar,
  },

  data: () => ({
    
  }),
};
</script>
