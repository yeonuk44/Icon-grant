<script>
import Create_Btn from '../Create_Btn';

export default {
  name: 'Survey',
  data: () => ({
      max: 0,
    }),
  components: {
      Create_Btn,
  }
}
</script>

<template>
 <v-content>
  <v-container fluid class="content" >
    <v-row justify="center" >
      <v-col
        sm="6"
        cols="12"
      >
      <v-btn large>View Instructions</v-btn>
      <h3 class="mb-5">What is your favorite color for a bird?</h3>
        <v-text-field
          v-model="label"
          label="Example : Pink"
          class="interval"
        ></v-text-field>
        <h3 class="mb-5">Check this box if you like birds</h3>
          <v-checkbox v-model="disabled" ></v-checkbox>
        <h3 class="mb-5">On a scale of 1-10, how much do you like birds?</h3>
          <v-slider v-model="max" step="10" ticks="always" tick-size="4>"></v-slider>
        <h3 class="mb-5">Write a short essay describing your favorite bird</h3>
          <v-text-field label="Lorem ipsum..." class="interval"></v-text-field>
        <v-btn @click="submit">Submit</v-btn>
      </v-col>
    </v-row>
  </v-container>
  <Create_Btn/>
 </v-content>
</template>

<style scoped>
.content {
    width: 90%;
    border:black solid 0.1em ;
}
.interval {
    padding-top: 5%;
}
</style>