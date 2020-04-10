<template>
  <div>
    <div style="position: relative">
      <v-img src="../assets/bg.jpg" style="height: 80vh"></v-img>
      <div class="bg">
        <h1 class="display-3 white--text">Alder Dev</h1>
        <p
          class="headline mt-3 white--text text-center font-weight-light"
        >De site a aplicativos, tudo para seu negocio</p>
        <v-btn color="#FABD00" class="white--text">Conhecer mais</v-btn>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

import { Component } from "vue-property-decorator";

@Component({})
export default class HelloWorld extends Vue {}
</script>

<style lang="sass" scoped>
.bg
  position: absolute
  left: 50%
  top: 50%
  transform: translate(-50%, -50%)
  width: 100%
  height: 100%
  display: flex
  flex-direction: column
  justify-content: center
  align-items: center
  background-color: rgba(0, 0, 0, 0.7)
</style>