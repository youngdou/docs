<template>
  <v-stepper v-model="e6" vertical>
    <v-stepper-step step="1" v-bind:complete="e6 > 1">
      Select an app
      <small>Summarize if needed</small>
    </v-stepper-step>
    <v-stepper-content step="1">
      <v-card class="grey lighten-1 z-depth-1 mb-5" height="200px"></v-card>
      <v-btn primary light @click.native="e6 = 2">Continue</v-btn>
      <v-btn flat light>Cancel</v-btn>
    </v-stepper-content>
    <v-stepper-step step="2" v-bind:complete="e6 > 2">Configure analytics for this app</v-stepper-step>
    <v-stepper-content step="2">
      <v-card class="grey lighten-1 z-depth-1 mb-5" height="200px"></v-card>
      <v-btn primary light @click.native="e6 = 3">Continue</v-btn>
      <v-btn flat light>Cancel</v-btn>
    </v-stepper-content>
    <v-stepper-step step="3">Select an ad format and name ad unit</v-stepper-step>
    <v-stepper-content step="3">
      <v-card class="grey lighten-1 z-depth-1 mb-5" height="200px"></v-card>
      <v-btn primary light @click.native="e6 = 4">Continue</v-btn>
      <v-btn flat light>Cancel</v-btn>
    </v-stepper-content>
    <v-stepper-step step="4">View setup instructions</v-stepper-step>
    <v-stepper-content step="4">
      <v-card class="grey lighten-1 z-depth-1 mb-5" height="200px"></v-card>
      <v-btn primary light @click.native="e6 = 1">Continue</v-btn>
      <v-btn flat light>Cancel</v-btn>
    </v-stepper-content>
  </v-stepper>
</template>

<script>
  export default {
    data () {
      return {
        e6: 1
      }
    }
  }
</script>
