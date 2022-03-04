<template>
  <v-app>
    <v-app-bar app color="blue darken-3" class="white--text p-4">
      <div class="text-h4 text-left mb-3 font-weight-bold ml-2">Blogs</div>
      <v-spacer></v-spacer>
      <v-btn depressed class="mr-2" color="primary" @click="dialog = true">
        Create new Blog
      </v-btn>
    </v-app-bar>
    <v-main>
      <v-row justify="center">
        <v-dialog v-model="dialog" persistent max-width="600px">
          <v-card>
            <v-card-title>
              <span class="text-h5 font-weight-bold">Create New Blog</span>
            </v-card-title>
            <v-card-text>
              <v-row>
                <v-col class="" cols="12">
                  <v-text-field
                    label="Title of blog"
                    solo
                    required
                  ></v-text-field>
                </v-col>
                <v-col class="py-0 my-0" cols="12">
                  <v-text-field
                    label="Author name"
                    required
                    solo
                  ></v-text-field>
                </v-col>
                <v-col class="pt-1 pb-2" cols="12">
                  <v-textarea solo label="Content"></v-textarea>
                </v-col>
              </v-row>
            </v-card-text>
            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn color="error" @click="dialog = false"> Cancel </v-btn>
              <v-btn color="success" @click="dialog = false"> Create </v-btn>
            </v-card-actions>
          </v-card>
        </v-dialog>
      </v-row>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    dialog: false,
  }),

  methods: {},
};
</script>
