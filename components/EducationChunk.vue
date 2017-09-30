<template>
<Chunk class="edu-chunk" title="Education">
    <div class="edu-block">
        <div class="edu-flex">
            <Thumbnail class="thumbnail" src="https://career.ucsd.edu/_images/UCSDlibrary.gif" alt="UCSD" />
            <div class="caption-wrapper">
                <div class="caption">
                    PhD Student
                </div>
            </div>
        </div>
        <div class="year">
            2017-Now
        </div>
    </div>
    <div class="edu-block">
        <div class="edu-flex">

            <Thumbnail class="thumbnail" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/RIT_Lettermark.svg/1280px-RIT_Lettermark.svg.png" alt="UCSD"/>
            <div class="caption-wrapper">
                <span class="caption">
                    B.S. Software<br/>Engineering
                </span>
            </div>
        </div>
        <div class="year">
            2012-2017
        </div>
    </div>
</Chunk>
</template>

<style scoped>
.edu-chunk {
    margin-bottom: -1rem;
}
.edu-block {
    position: relative;
    flex-basis: 15rem;
  flex-grow: 1;
  flex-shrink: 0;

  box-shadow: 0 0 1px gray;
  padding-left: .5rem;
  padding-top: .5rem;
    margin: 0 .5rem 1rem .5rem;

}
.edu-flex{
  /*
  background: rgba(0,0,0,.1);
  border-left: 3px solid rgba(0,0,0,.3);
  */

  
  display: flex;
  align-items: center;
  flex-direction: row;
}

.edu-flex>.thumbnail {
    height: 7rem;
    width: 7rem;
    flex-shrink: 0;
}
.edu-flex>.caption-wrapper {
    flex-grow: 1;
    text-align: center;
}
.caption-wrapper>.caption {
    display: inline-block;
    text-align: left;
}
.edu-block>.year {
    text-align: center;
    font-size: .8rem;
    opacity: .7;
    padding-bottom: .5rem;
}
</style>

<script>
import Chunk from '~/components/Chunk.vue'
import Thumbnail from '~/components/Thumbnail.vue'

export default {
  components: {
    Chunk,
    Thumbnail
  }
}
</script>