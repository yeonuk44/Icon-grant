<template>
  <v-app>

    <v-content>
      <!-- <AppBar/> -->
      <!-- <HelloWorld/> -->
      <!-- <MainPage/> -->
      <Tasks_AppBar/>
      <!-- <Tasks_main/> -->
      <Survey/>
    </v-content>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld';
// import AppBar from './components/AppBar';
// import MainPage from './components/MainPage';
// import Tasks_main from './components/Tasks_main';
import Tasks_AppBar from './components/Tasks_AppBar';
import Survey from './forms/Survey/Survey';

export default {
  name: 'App',

  components: {
    // HelloWorld,
    // AppBar,
    // MainPage,
    // Tasks_main,
    Tasks_AppBar,
    Survey,
  },

  data: () => ({
    
  }),
};
</script>
