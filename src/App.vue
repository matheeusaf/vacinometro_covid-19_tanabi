<template>
  <v-app>
    <v-app-bar app color="grey lighten-4" dark>
      <div class="d-flex align-center">
        <v-img alt="Coronavirus Logo" class="shrink mr-2" contain
          :src="require('../src/assets/coronavirus.png')" transition="scale-transition" width="40" />

        <v-img alt="Coronavirus logo letters" class="shrink mt-1 hidden-sm-and-down" contain min-width="100"
          :src="require('../src/assets/coronavirus-letters-logo.png')" width="100" />
      </div>

      <v-spacer></v-spacer>

      <v-btn color="blue darken-4" href="https://tanabi.sp.gov.br/" target="_blank" text>
        <span class="mr-2">Tanabi</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <HomePage />
    </v-main>
  </v-app>
</template>

<script>
  import HomePage from './components/HomePage';

  export default {
    name: 'App',

    components: {
      HomePage
    },

    data: () => ({
      //
    }),
  };
</script>