<template>
  <v-container fluid grid-list-md>
    <v-layout row wrap>
      <v-flex d-flex xs12 sm6 md4>
        <v-card color="grey darken-3" dark>
          <v-card-media src="/foto51.png" height="380px" >
          </v-card-media>
          
        </v-card>
      </v-flex>
      <v-flex d-flex xs12 sm6 md3>
        <v-layout row wrap>
          <v-flex d-flex>
            <v-card color="grey darken-2" dark>
             <v-card-title primary class="title">Борис Исаевич Нуриев</v-card-title>
             <v-card-text><p>Этот сайт посвящен легендарному советскому российскому нефтянику Борису Исаевичу Нуриеву. 
               </p></v-card-text>
            </v-card>
          </v-flex>
          
        </v-layout>
      </v-flex>
      
          </v-layout>
  </v-container>
</template>

<script>
import Carousel from '@/components/Carousel'

export default {
   components: {
     Carousel
   },
   data: () => ({
      lorem: `Lorem ipsum dolor sit amet, mel at clita quando. Te sit oratio vituperatoribus, nam ad ipsum posidonium mediocritatem, explicari dissentiunt cu mea. Repudiare disputationi vim in, mollis iriure nec cu, alienum argumentum ius ad. Pri eu justo aeque torquatos.`
   })
}
</script>
