<template>
  <div class="work-item">
      <slot name="thumbnail" />
      <div class="text">
          <a :href="src" class="title subtle">{{title}}</a>
      <div class="description">
          <slot/>
      </div>
      </div>
  </div>
</template>

<style lang="scss">
.work-item {
    width: 100%;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    .thumbnail {
        flex-basis: 5rem;
        flex-shrink: 0;
        flex-grow: 1;
    }
    .text {
        border-left: 2px solid #888;
        padding-left: 1rem;
        flex-basis: 80%;
        flex-grow: 1;
        flex-shrink: 0;
    }
    .title {
        font-weight: bold;
    }
}
a.subtle {
    color: inherit;
    text-decoration: none;
}
a.subtle:visited {
    color: #888;
}
a.subtle:link:hover, a.subtle:visited:hover {
    text-decoration: underline;
}
</style>




<script>
export default {
  props: ['title', 'src']
}
</script>
