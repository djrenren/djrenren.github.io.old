<template>
<Chunk class="quote-chunk">
    <div class="quote">
        <div class="quote-body">
            <div v-if="text" class="quote-text">{{text}}</div>
            <div v-if="attribution" class="quote-attribution">{{attribution}}</div>
        </div>
    </div>
</Chunk>
</template>

<style scoped>
.quote {
    width: 100%;
    background: rgba(0,0,0,.1);
    border-left: 3px solid rgba(0,0,0,.3);
    padding: .25rem .25rem;
    position: relative;
    text-align: center;
}

.quote-body {
    display: inline-block;
    margin: 0 auto;
    text-align: left;
}

.quote-text {
    font-style: italic;
}

.quote-attribution {
    margin-top: 1rem;
    opacity: .6;
    font-size: .7rem;
    text-align: right;
}
</style>

<script>
import Chunk from '~/components/Chunk.vue'

export default {
  components: {
    Chunk
  },
  props: ['text', 'attribution']
}
</script>