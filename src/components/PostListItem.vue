<template>
  <div class="col-md-8">
    <div class="post-item">
      <h1>{{ post.title }}</h1>
      <p>{{ post.body }}</p>
      <button class="btn btn-outline-primary">Show More</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "PostListItem",
  props: {
    post: Object,
  },
};
</script>

<style scoped>
.post-item {
  padding: 1rem;
  margin-bottom: 18px;
  border-radius: 6px;
  border: 1px solid #dddddd;
}
</style>