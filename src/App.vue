<template>
  <div class="container">
    <img src="@/assets/main-image.jpg" alt="Main Image" class="main-image">
    <div class="share-buttons">
      <IconX />
      <a href="https://mastodon.social/share" target="_blank">Mastodon</a>
      <a href="https://bsky.app/share" target="_blank">Bluesky</a>
      <a href="https://threads.net/share" target="_blank">Threads</a>
      <a href="https://line.me/share" target="_blank">LINE</a>
    </div>
  </div>
</template>

<script>
import IconX from './components/icons/iconX.vue'
import Sharebuttons from './components/ShareButtons.vue'

export default {
  name: 'App',
  components: {
    IconX
  }
}
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  text-align: center;
  padding: 20px;
  max-width: 1000px;
  margin: 0 auto;
}

.main-image {
  max-width: 100%;
  height: auto;
}

.share-buttons {
  display: flex;
  gap: 20px;
  margin-top: 20px;
}

.share-buttons a {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 64px;
  height: 64px;
  text-decoration: none;
  color: #000;
}
</style>