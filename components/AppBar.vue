<script>
  export default {
    name: 'AppBar',
    data:()=>({
        justify: [
            'start',
            'end',
            'center',
            'space-between',
            'space-around',
        ]
    })
  }
</script>

<template>
  <div>
    <v-app-bar
      color="#000000"
      dense
      dark
      height="70em"


    >
      
      <v-app-bar-nav-icon
      width="46 em">
          <v-icon >
          </v-icon>
      </v-app-bar-nav-icon>

      <v-toolbar-title> 
          <p class="display-1">
          Studec</p></v-toolbar-title>


      
    </v-app-bar>
  </div>
</template>