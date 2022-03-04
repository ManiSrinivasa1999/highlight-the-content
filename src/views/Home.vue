<template>
  <v-container fluid class="mt-4">
    <v-row class="pt-4">
      <v-col cols="12" md="3" v-for="n in 10" :key="n">
        <v-container class="py-0">
          <BlogPost />
        </v-container>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import BlogPost from "../components/BlogPost.vue";

export default {
  name: "Home",
  components: { BlogPost },
};
</script>
