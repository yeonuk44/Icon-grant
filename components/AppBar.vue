<script>
export default {
  name: "AppBar",
  data: () => ({
    justify: ["start", "end", "center", "space-between", "space-around"]
  })
};
</script>

<template>
  <div>
    <v-app-bar class="appbar" color="#000000" dense dark height="70em">
      <v-app-bar-nav-icon>
        <v-img :src="require('../assets/create.png')" contain width="4em" height="4em" />
      </v-app-bar-nav-icon>
      <v-toolbar-title>
        <p class="text display-1">Studec</p>
      </v-toolbar-title>
    </v-app-bar>
  </div>
</template>

<style scoped>
.appbar{
    padding-left: 45%;
}
.text{
    margin-top: 20%;
}
</style>