<template>
  <div class="content-container flex-1 p-5">
    <ContentItem
      :content="content"
      v-for="content of contents"
      :key="content.name"
    />
  </div>
</template>

<script>
import ContentItem from "./contentItem.vue";

export default {
  name: "contentContainer",

  components: {
    ContentItem,
  },
  props: {
    SportName: String,
  },

  data() {
    return {
      contents: [],
    };
  },
  watch: {
    SportName() {
      this.getNews();
    },
  },
  methods: {
    async getNews() {
      const apiKey = "08c960127df349ee90b743de972ebced";

      const name = this.SportName;

      const response = await fetch(
        `https://newsapi.org/v2/everything?q=${name}&excludeDomains=s.secure.espncdn.com
&rom=2021-07-23&sortBy=relevancy&apiKey=${apiKey}`
      );
      const data = await response.json();
      this.contents = data.articles;
      console.log(this.contents);
    },
  },
  mounted() {
    this.getNews();
  },
};
</script>

<style>
.content-container {
  overflow-y: scroll;
  height: 73vh;
}
</style>
