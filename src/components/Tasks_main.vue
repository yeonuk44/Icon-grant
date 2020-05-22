<template>
  <v-app>

    <v-content>
      <HelloWorld/>
      <v-container>
              <!-- <v-row class="text-center"> -->
              <v-row>

                <v-col>
                  <h2 class="mb-4">Select a customizable template to start a new project</h2>
                  <div>
                    <v-data-table
                    :dense="dense"
                    :fixed-header="fixedHeader"
                    :height="height"
                    :headers="headers"
                    :items="kind"
                    class="table"
                    >
                    <!-- <template v-slot:default>
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


                    </template> -->
                    </v-data-table>
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
    dense:false , //줄간격 만들기
    fixedHeader:false,
    heght:100,
    headers: [
      {
        align:'start',
        sortable:false,
        value:'name',
      },
      {text:'Index', value:'index'},
      {href:'Survey', value :'survey'},
      {text:'Vision', value:'vision'},
      {text:'Language', value:'language'},
      {text:'Other', value:'other'},
    ],

    kind: [
      {
        index:0,
        survey:'Survey link',
        vision:'Image Classification',
        language:'Sentiment Analysis',
        other:'Data Collection',
      },
      {
        index:1,
        survey:'Survey',
        vision:'Bounding Box',
        language:'Intent Detection',
        other:'Website Collection',
      },
      {
        index:2,
        vision:'Semantic Segmentation',
        language:'Collect Utterance',
        other:'Website Classification',
      },
      {
        index:3,
        vision:'Instance Segmentation',
        language:'Emotion Detection',
        other:'Item Equality',
      },
      {
        index:4,
        vision:'Polygon',
        language:'Semantic Similarity',
        other:'Search Relevance',
      },
      {
        index:5,
        vision:'Keypoint',
        language:'Audio Transcription',
        other:'Other',
      },
      {
        index:6,
        vision:'Image Contains',
        language:'Conversation Relevance',
      },
      {
        index:7,
        vision:'Video Classification',
        language:'Document Classification',
      },
      {
        index:8,
        vision:'Moderation of an Image',
        language:'Translation Quality',
      },
      {
        index:9,
        vision:'Image Tagging',
        language:'Audio Naturalness',
      },
      {
        index:10,
        vision:'Image Summatiazation',
      },
    ],
   
    
  }),
};
</script>
