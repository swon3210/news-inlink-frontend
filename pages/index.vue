<template>
  <v-container fill-height>
    <v-row
      class="flex-child ma-0"
    >
      <v-col
        class="d-flex"
        cols="12"
      >
        <v-row>
          <v-col cols="12">
            <v-sheet
              class="d-flex"
              color="white lighten-3"
              height="1000"
              :elevation="2"
            >
              
            </v-sheet>
          </v-col>
          <!-- <v-col cols="6">
            <v-sheet
              class="d-flex"
              color="green lighten-3"
              height="200"
            >
            </v-sheet>
          </v-col>
          <v-col cols="6">
            <v-sheet
              class="d-flex"
              color="yellow lighten-3"
              height="200"
            >
            </v-sheet>
          </v-col> -->
          <v-col>
            <div class="text-center">
              <v-pagination
                v-model="page"
                :length="6"
              ></v-pagination>
            </div>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
    
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      page: 1,
    }
  },
  components: {

  }
}
</script>
