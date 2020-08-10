<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-dark">
    <div class="container">
      <div class="collapse navbar-collapse">
        <ul class="navbar-nav justify-nav mr-auto">
          <li class="nav-item">
            <a class="btn btn-primary" href="#">Write a Post</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
.justify-nav {
  width: 100%;
  justify-content: flex-end;
}
</style>