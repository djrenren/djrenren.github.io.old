<template>
  <Chunk class="pub-chunk" title="Publications">
    <Publication
      title="Constant-Time WebAssembly"
      authors="John Renner, Sunjay Cauligi, Deian Stefan"
      src="https://github.com/djrenren/djrenren.github.io/releases/download/wasm-review/main.pdf" />
  </Chunk>
</template>

<style scoped>
.pub-chunk {
    color: #888;
}
</style>

<script>
import Chunk from '~/components/Chunk'
import Publication from '~/components/Publication'
export default {
  components: {
    Chunk,
    Publication
  }
}
</script>
