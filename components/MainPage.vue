<script>
  export default {
    name: 'MainPage'
  }
</script>

<template>
  <v-container>
    <v-row class="text-center"> 
      <v-col class="mb-4">
        <h1 class="display-1 font-weight-bold mb-3">
          Get Started with Mechanical Turk
        </h1>

      </v-col>

      <v-col
        cols="12"
      >
        <v-row justify="center">
            <v-row justify="center">
                <v-col justify="center">
                <v-img
                    :src="require('../assets/create.png')"
                    class="my-3"
                    contain
                    height="200"/>
                <p class="headline ">Create Tasks</p>
                <p class="body-1">Human intelligence through an API. Access a<br/> global, on-demand, 24/7 workforce.</p>
                <div class="my-2">
                <v-btn color="#E6EE9C">Create a Requester account</v-btn>
                </div>
                </v-col>
            </v-row>
            <v-col>
            <v-icon x-large></v-icon>
            <p class="headline ">or</p>
            </v-col>
            <v-row justify="center">
                <v-col justify="center">
                <v-img
                    :src="require('../assets/make.png')"
                    class="my-3"
                    contain
                    height="200"/>
                <p class="headline ">Make Money</p>
                <p class="body-1">Make money in your spare time. Get paid for<br/> completing simple tasks.</p>
                <div class="my-2">
                <v-btn color="#E6EE9C">Create a Worker account</v-btn>
                </div>  
                </v-col>
            </v-row>
        
         
        </v-row>
      </v-col>

    </v-row>
  </v-container>
</template>
