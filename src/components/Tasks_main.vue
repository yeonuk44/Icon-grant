<template>
  <v-app>

    <v-content>
      <HelloWorld/>
      <v-container>
              <!-- <v-row class="text-center"> -->
              <v-row>

                <v-col cols="12">
                  <h2 class="mb-4">Select a customizable template to start a new project</h2>
                  <div>
                    <v-simple-table
                    :dense="dense"
                    :fixed-header="fixedHeader"
                    :height="height"
                    >
                    <template v-slot:default>
                    <thead>
                      <tr>
                        <th class="text-left">Survey</th>
                      </tr>
                    </thead>
                    <tbody>
                      <tr v-for = "item in Survey_option" :key="item.kind">
                        <td>{{ item.kind}}</td>
                      </tr>
                    </tbody>


                    <thead>
                      <tr>
                        <th class="text-left">Vision</th>
                      </tr>
                    </thead>
                    <tbody>
                      <tr v-for = "item in Vision_option" :key="item.kind">
                        <td>{{ item.kind}}</td>
                      </tr>
                    </tbody>


                    <thead>
                      <tr>
                        <th class="text-left">Language</th>
                      </tr>
                    </thead>
                    <tbody>
                      <tr v-for = "item in Language_option" :key="item.kind">
                        <td>{{ item.kind}}</td>
                      </tr>
                    </tbody>

                    <thead>
                      <tr>
                        <th class="text-left">Other</th>
                      </tr>
                    </thead>
                    <tbody>
                      <tr v-for = "item in Other_option" :key="item.kind">
                        <td>{{ item.kind}}</td>
                      </tr>
                    </tbody>


                    </template>
                    </v-simple-table>
                  </div>


                </v-col>
              </v-row>
      </v-container>

    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './HelloWorld';

export default {
  name: 'App',

  components: {
    HelloWorld,
  },

  data: () => ({
    dense:false,
    fixedHeader:false,
    heght:300,
    Survey_option: [
      {
        kind:'Survey link'
      },
      {
        kind:'Survey'
      },
    ],
    Vision_option: [
      {
        kind:'Image Classification'
      },
      {
        kind:'Bounding Box'
      },
      {
        kind:'Semantic Segmentation'
      },
      {
        kind:'Instance Segmentation'
      },
      {
        kind:'Polygon'
      },
      {
        kind:'Keypoint'
      },
      {
        kind:'Image Contains'
      },
      {
        kind:'Video Classification'
      },
      {
        kind:'Moderation of an Image'
      },
      {
        kind:'Image Tagging'
      },
      {
        kind:'Image Summatiazation'
      },
    ],
    Language_option: [
      {
        kind:'Sentiment Analysis'
      },
      {
        kind:'Intent Detection'
      },
      {
        kind:'Collect Utterance'
      },
      {
        kind:'Emotion Detection'
      },
      {
        kind:'Semantic Similarity'
      },
      {
        kind:'Audio Transcription'
      },
      {
        kind:'Conversation Relevance'
      },
      {
        kind:'Document Classification'
      },
      {
        kind:'Translation Quality'
      },
      {
        kind:'Audio Naturalness'
      },
    ],
    Other_option: [
      {
        kind:'Data Collection'
      },
      {
        kind:'Website Collection'
      },
      {
        kind:'Website Classification'
      },
      {
        kind:'Item Equality'
      },
      {
        kind:'Search Relevance'
      },
      {
        kind:'Other'
      },
    ]
  }),
};
</script>
