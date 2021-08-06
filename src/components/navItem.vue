<template>
  <div
    @click="getInfo"
    class="filter-item py-10 px-0 mx-5 flex items-center justify-start cursor-pointer"
  >
    <img :src="item.image" alt="item1" class="mx-5" />
    <h3 class="flex-1 text-xl break-words font-bold">{{ item.name }}</h3>
  </div>
</template>

<script>
export default {
  name: "navItem",
  props: {
    item: Object,
  },
  data() {
    return {};
  },
  methods: {
    getInfo() {
      this.$emit("name-from-nav", this.item.name);
    },
  },
};
</script>

<style>
.filter-item {
  transition: 0.5s all ease-in-out;
}
h3 {
  font-family: "Oswald", sans-serif;
  /* color: rgb(0, 35, 97); */
}
.filter-item:hover {
  background: rgba(0, 35, 97);
  color: white;
}
</style>
