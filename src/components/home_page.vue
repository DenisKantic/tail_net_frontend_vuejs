<template>
  <v-app>
    <Navigation />
    <br />
    <br />
    <br />
    <v-container class="mt-6" style="padding: 0 16rem">
      <v-row>
        <!-- Left Sidebar (Profile Info) -->
        <v-col cols="12" md="3">
          <LeftProfileCard />
        </v-col>

        <!-- Center Column (Main Feed) -->
        <v-col cols="12" md="6">
          <CreateUserPost />
          <MainFeed />
        </v-col>

        <!-- Right Sidebar (Promotions / Ads) -->
        <v-col cols="12" md="3">
          <v-card class="pa-3">
            <v-card-title>Sponsored</v-card-title>
            <v-divider class="my-3"></v-divider>
            <p>Advertisement content...</p>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script lang="ts">
import Navigation from '@/views/navigation_bar/navigation_bar.vue'
import LeftProfileCard from './home_page_components/left_profile_card/user_card.vue'
import MainFeed from './home_page_components/main_feed/main_feed.vue'
import CreateUserPost from './create_post/user_post.vue'

export default {
  components: {
    Navigation,
    LeftProfileCard,
    MainFeed,
    CreateUserPost,
  },
}
</script>
