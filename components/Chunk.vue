<template>
    <section class="chunk">
        <div class="container">
            <div v-if="title" class="title">{{ title }}</div>
            <div class="content">
                <slot></slot>
            </div>
        </div>
    </section>
</template>

<style scoped>
.container {
    max-width: 680px; 
    margin: 0 auto; 
    padding: 1rem .5rem;
}
.container > .title {
    text-transform: uppercase;
    color: #009999;
    margin-bottom: 1rem;
}

.container .content {
    display: flex;
    justify-content: center;
    flex-wrap:wrap;
}
</style>

<script>
export default {
  props: ['title']
}
</script>