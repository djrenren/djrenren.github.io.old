<template>
  <Chunk class="work-chunk" title="Previous Work">
      <WorkItem title="Kythe Language Server" src="https://github.com/google/kythe/tree/master/kythe/go/languageserver">
        <thumbnail class="thumbnail" slot="thumbnail" src="/vscode.png" alt="VSCode Logo" />
          Implemented a Language Server capable of providing local cross-references and type information supplied by Kythe’s static index.
          My work was incorporated into the default workstation config at Google.
      </WorkItem>
      <WorkItem title="Rust Indexer for Kythe" src="https://github.com/google/kythe/tree/master/kythe/rust">
        <thumbnail class="thumbnail" slot="thumbnail" src="https://www.rust-lang.org/logos/rust-logo-blk.svg" alt="Rust Logo" />
          Designed and built a tool for indexing cross-references in Rust code using the Kythe knowledge graph protocols, enabling definition lookups and codesearch.
      </WorkItem>
      <WorkItem title="Facebook Cache Monitoring">
        <thumbnail class="thumbnail" slot="thumbnail" src="/fb.png" alt="Facebook Logo" />
            Created a service for determining and alerting on realtime cache consistency for Facebook’s whole memcache and TAO deployment.
      </WorkItem>
  </Chunk>
</template>

<style scoped>
.pub-chunk {
    color: #888;
}

.work-chunk .work-item:not(:first-child) {
    margin-top: 1rem;
}
</style>

<script>
import Chunk from '~/components/Chunk'
import WorkItem from '~/components/WorkItem'
import Thumbnail from '~/components/Thumbnail.vue'

export default {
  components: {
    Chunk,
    WorkItem,
    Thumbnail
  }
}
</script>
