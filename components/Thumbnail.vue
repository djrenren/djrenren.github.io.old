<template>
  <div :style="{background: `url(${src})`, backgroundSize: 'contain', backgroundPosition: 'center', backgroundRepeat: 'no-repeat'}" :aria-label="alt">
  </div>
</template>

<script>
export default {
  props: ['src', 'alt']
}
</script>