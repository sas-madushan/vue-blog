<template>
  <div id="app">
    <Header />
    <div class="container">
      <PostList :posts="posts" />
    </div>
  </div>
</template>

<script>
import Header from "./components/Header";
import PostList from "./components/PostList";

export default {
  name: "App",
  components: {
    Header,
    PostList,
  },
  data: function () {
    return {
      posts: [],
    };
  },
  mounted: function () {
    const baseUrl = `https://jsonplaceholder.typicode.com/posts`;
    fetch(baseUrl)
      .then((response) => response.json())
      .then((posts) => (this.posts = posts));
  },
};
</script>

<style>
</style>
