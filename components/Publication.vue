<template>
  <div class="publication-item">
      <a :href="src" class="title">{{title}}</a>
      <p>{{authors}}</p>
  </div>
</template>

<style lang="scss">
.publication-item {
    width: 100%;
    padding-left: 0.5rem;
    .title {
        color: black;
        font-weight: bold;
    }
}
</style>

<script>
export default {
  props: ['title', 'authors', 'src']
}
</script>
