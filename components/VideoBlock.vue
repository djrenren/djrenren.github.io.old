<template>
  <a :href="src" class="video-block" :style="{background: `url(${previewImage})`, backgroundSize: 'cover'}">
    <div class="title">
        {{title}}
        <div class="source">{{domain}}</div>
    </div>

  </a>
</template>

<style scoped>
.video-block {
    height: 162px;
    width: 45%;
    position: relative;
}
.video-block>.title {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    padding: .5rem 1rem;
    background: radial-gradient(rgba(0,0,0,.3) 60%, rgba(0,0,0,.4));
    color: white;
    transition: padding .25s;
}

.video-block>.title>.source {
    font-size: .6rem;
    opacity: .7;
    left: 1rem;
}
.video-block:hover>.title {
    padding-bottom: 1.25rem;
}
</style>

<script>
export default {
  props: ['src', 'title', 'previewImage'],
  computed: {
    domain () {
      let start = this.src.indexOf('//') + 2
      let end = this.src.indexOf('/', start)
      if (end === -1) end = this.src.length
      return this.src.substring(start, end)
    }
  }
}
</script>
