<template>
  <div class="flex my-10  justify-between divide-y divide-gray-300">
    <img class="w-1/4 object-cover" :src="content.urlToImage" alt="" />

    <div class="flex-1 flex flex-col px-10 py-5">
      <h2 class="text-3xl mb-3">{{ content.title }}</h2>
      <p class="text-lg flex-1">
        {{ content.description }}
      </p>
      <button class="view-detail-btn self-end">Read Full Article</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "contentItem",
  props: {
    content: Object,
  },
};
</script>

<style>
p {
  font-family: "Open Sans", sans-serif;
}

.view-detail-btn {
  background: rgb(0, 35, 97);
  color: white;
  padding: 0.5rem;
  border-radius: 5px;
  font-family: "Oswald", sans-serif;
  transition: 0.2s all ease-in-out;
}

.view-detail-btn:hover {
  transform: scale(1.05);
}
</style>
