<template>
  <!-- Center Column (Main Feed) -->

  <!-- Loop through posts and display them -->
  <v-card v-for="(post, index) in posts" :key="index" class="pa-3 mb-3">
    <v-card-title>{{ post.title }}</v-card-title>
    <v-card-subtitle>{{ post.author }}</v-card-subtitle>
    <v-card-text>{{ post.content }}</v-card-text>
  </v-card>
</template>

<script lang="ts">
export default {
  data() {
    return {
      posts: Array.from({ length: 10 }, (_, i) => ({
        title: `Post ${i + 1}`,
        author: `Author ${i + 1}`,
        content: `This is the content of post ${i + 1}.`,
      })),
    }
  },
}
</script>
