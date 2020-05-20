<script>
export default {
  name: 'Tasks_AppBar',
}
</script>
<template>
  <div>
    <v-app-bar
      class="appBar"
      color="#000000"
      dense
      dark
    >
      <v-app-bar-nav-icon>
         <v-img :src="require('../assets/create.png')" contain width="4em" height="3em" />
      </v-app-bar-nav-icon>

      <v-toolbar-title class="title">Studec</v-toolbar-title>
      <v-btn text>Create</v-btn>     
      <v-btn text>Manage</v-btn>
      <v-btn text>Developer</v-btn>

      <v-spacer></v-spacer>
      <v-btn text small>User Name</v-btn>     
      <v-btn text small>Sign Out</v-btn>
      <v-btn text small>Help</v-btn>

    
      <!-- <v-menu
        left
        bottom
      >
        <template v-slot:activator="{ on }">
          <v-btn icon v-on="on">
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </template>

        <v-list>
          <v-list-item
            v-for="n in 5"
            :key="n"
            @click="() => {}"
          >
            <v-list-item-title>Option {{ n }}</v-list-item-title>
          </v-list-item>
        </v-list> 
      </v-menu> -->
    </v-app-bar>

  <p class="appBar" >New Project </p>
  </div>
</template>

<style scoped>
.appBar {
  padding-left: 5%;
}
.title{
  margin-right: 2em;
}
</style>