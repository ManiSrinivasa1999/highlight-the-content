<template>
  <v-card class="mx-auto" color="blue" dark>
    <v-card-title>
      <span class="text-h6 font-weight-bold">Title of Blog</span>
    </v-card-title>

    <v-card-text class="text-h5 font-weight-bold">
      "Turns out semicolon-less style is easier and safer in TS because most
      gotcha edge cases are type invalid as well."
    </v-card-text>

    <v-card-actions>
      <v-list-item class="grow">
        <v-list-item-avatar color="grey darken-3">
          <v-img
            class="elevation-6"
            alt=""
            src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
          ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title>Evan You</v-list-item-title>
        </v-list-item-content>

        <v-row align="center" justify="end">
          <v-icon class="mr-1"> mdi-pencil </v-icon>
          <v-icon class="mr-1"> mdi-delete </v-icon>
        </v-row>
      </v-list-item>
    </v-card-actions>
  </v-card>
  <!-- <v-card class="mx-auto">
    <v-list-item three-line>
      <v-list-item-content>
        <div class="text-overline mb-4">Author Name</div>
        <v-list-item-title class="text-h5 mb-1">
          Title of Blog
        </v-list-item-title>
        <v-list-item-subtitle
          >Lorem ipsum dolor sit amet consectetur, adipisicing elit. Totam sunt
          sequi praesentium suscipit autem soluta expedita. Laboriosam, corrupti
          voluptate harum molestiae, libero aspernatur placeat voluptatibus
          dicta aperiam, modi ad quaerat!</v-list-item-subtitle
        >
      </v-list-item-content>
    </v-list-item>

    <v-card-actions>
      <v-spacer></v-spacer>
      <v-btn color="primary" class="ma-2 white--text"> Edit </v-btn>
      <v-btn color="error" class="ma-2 white--text"> Delete </v-btn>
    </v-card-actions>
  </v-card> -->
</template>

<script>
// @ is an alias to /src

export default {
  name: "BlogPost",
  components: {},
};
</script>
