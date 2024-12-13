<script>
    import IconX from './icons/iconX.vue'
    export default {
        name: 'ShareButtons',
        components: {
            IconX
        }
    }  
</script>

<template>
  <div class="share-buttons">
    <IconX />
    <a href="https://mastodon.social/share" target="_blank">Mastodon</a>
    <a href="https://bsky.app/share" target="_blank">Bluesky</a>
    <a href="https://threads.net/share" target="_blank">Threads</a>
    <a href="https://line.me/share" target="_blank">LINE</a>
  </div>
</template>

<style scoped>
.share-buttons {
  margin-top: 20px;
  justify-content: center;
  align-items: center;
}
</style>