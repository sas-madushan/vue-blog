<template>
  <div class="row">
    <ResultEmpty v-if="posts.length === 0" />
    <PostListItem v-for="post in posts" v-bind:key="post.id" :post="post" />
  </div>
</template>

<script>
import PostListItem from "./PostListItem";
import ResultEmpty from "./ResultEmpty";

export default {
  props: {
    posts: {
      type: Array,
    },
  },
  components: {
    PostListItem,
    ResultEmpty,
  },
  name: "PostList",
};
</script>