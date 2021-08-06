<template>
  <div class="flex m-10 items-center justify-center">
    <img id="logo" class="m-4" src="../assets/logo.png" alt="logo" />
    <h1 class="text-5xl">Tokyo Olympic Games News Update</h1>
  </div>
  <div class="flex">
    <NavSection @sport-name="SportName = $event" />
    <ContentContainer :SportName="SportName" />
  </div>
</template>

<script>
import NavSection from "../components/navSection.vue";
import ContentContainer from "../components/contentContainer.vue";

export default {
  name: "Home",
  components: {
    NavSection,
    ContentContainer,
  },
  data() {
    return {
      SportName: "Archery",
    };
  },
  methods: {},
};
</script>

<style>
#logo {
  width: 20em;
  margin-right: 5em;
}
h1 {
  font-family: "Oswald", sans-serif;
  color: rgb(0, 35, 97);
}
</style>
