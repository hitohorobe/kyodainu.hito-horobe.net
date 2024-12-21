<template>
  <div class="container">
    <header>
      <h1>巨大な犬、巨犬（きょだいぬ）</h1>
    </header>
    <div class="main">
      <img src="/main-image.jpg" alt="Main Image" class="main-image" />
      <div class="description">
        <p>Share "巨大な犬、巨犬（きょだいぬ）"</p>
      </div>
      <div class="share-buttons">
        <IconX />
        <IconMastodon />
        <iconMisskey />
        <IconBluesky />
        <IconLine />
        <iconShareAPI />
      </div>
    </div>
    <footer>
      <p><a href="https://x.com/hito_horobe2">@hito_horobe2</a></p>
    </footer>
  </div>
</template>

<script>
import IconX from './components/icons/iconX.vue'
import IconMastodon from './components/icons/iconMastodon.vue'
import iconMisskey from './components/icons/iconMisskey.vue'
import IconBluesky from './components/icons/iconBluesky.vue'
import IconLine from './components/icons/iconLine.vue'
import iconShareAPI from './components/icons/iconShareAPI.vue'

export default {
  name: 'App',
  components: {
    IconX,
    IconMastodon,
    iconMisskey,
    IconBluesky,
    IconLine,
    iconShareAPI,
  },
  setup() {
    return {
      title: '巨大な犬、巨犬（きょだいぬ）',
      text: '巨大な犬、巨犬（きょだいぬ）',
      url: 'https://kyodainu.hito-horobe.net/',
      imageName: 'main-image.jpg',
    }
  },
}
</script>

<style scoped>
.container {
  margin: 0;
}

.main {
  margin-top: 10px;
  text-align: center;
}

header {
  position: sticky;
  top: 0;
  width: 100%;
  background-color: #d0d7deb3;
  color: black;
  text-align: center;
  padding: 10px 0;
  margin: 0px;
  z-index: 1000;
}

header h1 {
  margin: 0;
  padding: 0;
  font-size: x-large;
}

.main-image {
  width: 100%;
  max-width: 600px;
  height: auto;
}

.share-buttons {
  margin: 20px 0;
}

.share-buttons a {
  text-decoration: none;
  color: #0073e6;
}

footer {
  background-color: #f1f1f1;
  text-align: center;
  padding: 10px 0;
  position: fixed;
  bottom: 0;
  width: 100%;
}

@media (max-width: 600px) {
  .main-image {
    width: 90%;
  }

  .share-buttons a {
    display: block;
    margin: 10px 0;
  }
}
</style>
