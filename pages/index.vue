<template>
    <div class="main-container">
      <HeaderChunk />
      <Chunk title="About Me">
        <div style="width: 100%; padding: 0 .5rem;">
          I'm a graduate currently pursuing my PhD in Computer Science at UCSD.
          Much of my work has been focused on programming languages.
          If for any reason you'd like to connect with me, please reach out to me via email.
        </div>
      </Chunk>
      <EducationChunk />
      <WorkChunk />
      <VideoChunk />
      <PublicationsChunk />
      <div style="flex-grow: 1; flex-shrink: 1;" />
      <Chunk style="color: #888; font-size: .7rem;">
        Copyright &copy; 2017 John Renner
      </Chunk>
    </div>
</template>

<script>
import Chunk from '~/components/Chunk.vue'
import HeaderChunk from '~/components/HeaderChunk.vue'
import QuoteChunk from '~/components/QuoteChunk.vue'
import VideoChunk from '~/components/VideoChunk.vue'
import EducationChunk from '~/components/EducationChunk.vue'
import WorkChunk from '~/components/WorkChunk.vue'
import PublicationsChunk from '~/components/PublicationsChunk.vue'

export default {
  components: {
    Chunk,
    HeaderChunk,
    QuoteChunk,
    EducationChunk,
    VideoChunk,
    PublicationsChunk,
    WorkChunk
  },
  head () {
    return {
      title: 'John Renner'
    }
  }
}
</script>

<style>

.main-container {
  display: flex;
  flex-direction: column;
  width: 100%;
  height: 100%;
}
.main-container>* {
  background: white;
}
</style>
