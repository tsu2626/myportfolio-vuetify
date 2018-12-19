<template>
  <v-app>
    <v-toolbar app>
      <v-toolbar-title class="headline text-uppercase">
        <v-btn
          flat
          href="http://localhost:8080/#/"
          target="_blank"
        >
        {{ title }}
        </v-btn>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-add-down">
        <v-btn flat>About</v-btn>
        <v-btn flat>Service</v-btn>
        <v-btn flat>Contact</v-btn>
      </v-toolbar-items>      
      <!-- <span class="mr-2">Latest Release</span> -->
    </v-toolbar>

    <v-content>
      <HelloWorld/>
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data () {
    return {
      title: 'Tsuyoshi'
    }
  }
}
</script>
