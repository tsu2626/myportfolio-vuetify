<template>
  <v-container>
    <v-layout
      text-xs-center
      wrap
    >
      <v-flex xs12>
        <v-img
          class="my-3"
          contain
          height="200"
        ></v-img>
      </v-flex>

      <v-flex mb-4>
        <h1 class="display-2 font-weight-bold mb-3">
          Welcome to Tsuyoshi Hirosawa's Portfolio Site
        </h1>
        <p class="">
          Web Engineer
        </p>
      </v-flex>

      <v-flex
        mb-5
        xs12
      >
        <h2 class="headline font-weight-bold mb-3">Share</h2>

        <v-layout justify-center>
          <a
            v-for="(content, i) in contents"
            :key="i"
            :href="content.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ content.text }}
          </a>
        </v-layout>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      contents: [
        {
          text: 'Twitter',
          href: 'http://twitter.com/share?url=http://http://localhost:8080/#/'
        },
        {
          text: 'Facebook',
          href: 'https://www.facebook.com/sharer/sharer.php?u=http://twitter.com/share?url=http://http://localhost:8080/#/'
        },
        {
          text: 'LINE',
          href: 'https://social-plugins.line.me/lineit/share?url=http://localhost:8080/#/'
        }

      ]
    })
  }
</script>

<style>

</style>
