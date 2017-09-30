<template>
    <Chunk class="header">
        <img class="photo" />
        <div class="info">
            <h1 class="name">
                John Renner 
            </h1>
            <p class="contact">
                <a href="mailto:john@jrenner.net" class="subtle"><i class="fa fa-envelope"></i> &nbsp;john@jrenner.net</a> &middot;
                <a href="//github.com/djrenren" class="subtle"><i class="fa fa-github"></i> djrenren</a>
            </p>
        </div>
    </Chunk>
</template>

<style lang="scss" scoped>
.fa {
    display: inline !important;
}
.header {
    background: #009999;
    color: white;
    box-shadow: 0 0 5px #AAA;
    z-index: 1;
}
.photo {
    display: block;
    width: 7rem;
    height: 7rem;
    flex-basis: content;
    border-radius: 50%;
    background: gray;
    margin: 0 1rem;
    background: url('/me.jpg');
    background-size: cover;
    background-position: center;
    border: 1px solid rgba(255,255,255,.6);
    box-shadow: inset 0 0 5px gray;
}

.info {
    flex-basis: content;
    align-self: center;
    text-align: center;
    font-size: .8rem;
    .contact {
        text-align: left;
        display: inline-block;
        width: 100%;
    }
    .name {
        font-size: 2rem;
    }
}

</style>

<script>
import Chunk from '~/components/Chunk.vue'

export default {
  components: {
    Chunk
  }
}
</script>