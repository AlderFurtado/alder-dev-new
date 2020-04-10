<template>
  <div class="home">
    <HelloWorld />
    <h1 class="display-5 font-weight-light mt-6 ml-12">Quem sou eu</h1>
    <AboutMe />
    <Timeline />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import AboutMe from "@/components/AboutMe.vue";
import Timeline from "@/components/Timeline.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
    AboutMe,
    Timeline
  }
};
</script>
