<template>
  <div>
    <h2 class="p-5 text-xl font-bold">Check the latest updates by sports:</h2>

    <div class="filter-section">
      <navItem
        v-for="item in SportsItems"
        :key="item.name"
        :item="item"
        @name-from-nav="$emit('sportName', $event)"
      />
    </div>
  </div>
</template>

<script>
import navItem from "./navItem.vue";
import SportsItems from "../../db/db.json";

export default {
  name: "navSection",
  components: {
    navItem,
  },

  data() {
    return {
      SportsItems,
    };
  },

  methods: {
    // SportName(event) {
    //   this.$emit("sport-name", event);
    // },
  },
};
</script>

<style>
.filter-section {
  overflow-y: scroll;
  height: 65vh;
}

h2 {
  font-family: "Oswald", sans-serif;
  color: rgb(0, 35, 97);
}
</style>
