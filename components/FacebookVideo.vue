<template>
<div class="fb-video" :data-href="url" data-width="500" data-show-text="false">
    <div class="fb-xfbml-parse-ignore">
        <blockquote :cite="url">
            <a :href="url">{{title}}</a>
            <p>{{title}}.</p>
        </blockquote>
    </div>
</div>
</template>

<script>
export default {
  props: ['url', 'title'],
  head: {
    script: [
      { src: '//connect.facebook.net/en_US/sdk.js#xfbml=1&version=v2.6' }
    ]
  }
}
</script>
