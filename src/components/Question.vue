<template>
  <v-container fluid>
    <v-row align="center">
      <v-col class="d-flex" cols="12" sm="6">
        <v-select :items="talks" label="Select talk" dense outlined></v-select>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12" sm="6" md="6">
        <v-text-field
          label="Email"
          placeholder="Write your email for getting answer."
          outlined
        ></v-text-field>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12" md="6">
        <v-textarea
          outlined
          name="questions"
          label="Questions"
          value="Write your questions"
        ></v-textarea>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    talks: ["A", "B", "C"]
  })
};
</script>
