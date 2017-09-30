<template>
    <Chunk class="video-chunk" title="talks">
        <video-block
            src="https://www.facebook.com/ssebot/videos/10154724915057736/"
            title="What Could Go Wrong?"
            previewImage="https://scontent.fsan1-1.fna.fbcdn.net/v/t15.0-10/18466877_10154725070422736_1955541082800390144_n.jpg?oh=ef33b2fb8996eae872b529c0b01639f3&oe=5A3DAC50"/>
        <video-block
            src="https://www.youtube.com/watch?v=KwnKRlzJlwc"
            title="Monads Mo Problems"
            previewImage="https://img.youtube.com/vi/KwnKRlzJlwc/0.jpg"/>
    </Chunk>
</template>

<style>
.video-chunk .content {
    flex-wrap: nowrap !important;
    justify-content:space-between;
}
.video-chunk .content::before {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: red;
}
.video-block {
    box-shadow: 0 0 5px grey;
}
.video-block:not(:first-child) {
    margin-left: 1rem;
}
</style>

<script>
import Chunk from '~/components/Chunk.vue'
import FacebookVideo from '~/components/FacebookVideo.vue'
import VideoBlock from '~/components/VideoBlock.vue'

export default {
  components: {
    Chunk,
    FacebookVideo,
    VideoBlock
  }
}
</script>