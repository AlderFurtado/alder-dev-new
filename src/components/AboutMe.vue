<template >
  <v-row justify="center">
    <v-col class="text-center" cols="12" md="5">
      <v-avatar color="grey" size="120">
        <v-img src="@/assets/alder.png"></v-img>
      </v-avatar>
      <h1 class="subtitle-1 mt-6 mx-6">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora, fugit. Sed,
        quae facilis. Asperiores dolor qui cumque, cupiditate ea quod eaque dolorem
        aliquid deleniti quisquam minima possimus consequuntur aut. Totam.
      </h1>
    </v-col>
  </v-row>
</template>

<script lang="ts">
import Vue from "vue";
import Component from "vue-class-component";

@Component({})
export default class AboutMe extends Vue {}
</script>