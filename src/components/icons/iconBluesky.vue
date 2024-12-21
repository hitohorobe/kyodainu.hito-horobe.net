<script>
export default {
  name: 'IconBluesky',
  setup() {
    const text = '巨大な犬、巨犬（きょだいぬ）'
    const siteUrl = 'https://kyodainu.hito-horobe.net/'
    const url = 'https://bsky.app/intent/compose?text=' + encodeURIComponent(text + '\n' + siteUrl)
    return { url }
  },
}
</script>

<template>
  <div class="icon-bluesky">
    <a v-bind:href="url" target="_blank">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 64 57"
        width="16"
        height="16"
        style="vertical-align: sub"
      >
        <path
          fill="white"
          d="M13.873 3.805C21.21 9.332 29.103 20.537 32 26.55v15.882c0-.338-.13.044-.41.867-1.512 4.456-7.418 21.847-20.923 7.944-7.111-7.32-3.819-14.64 9.125-16.85-7.405 1.264-15.73-.825-18.014-9.015C1.12 23.022 0 8.51 0 6.55 0-3.268 8.579-.182 13.873 3.805ZM50.127 3.805C42.79 9.332 34.897 20.537 32 26.55v15.882c0-.338.13.044.41.867 1.512 4.456 7.418 21.847 20.923 7.944 7.111-7.32 3.819-14.64-9.125-16.85 7.405 1.264 15.73-.825 18.014-9.015C62.88 23.022 64 8.51 64 6.55c0-9.818-8.578-6.732-13.873-2.745Z"
        ></path>
      </svg>
    </a>
  </div>
</template>

<style scoped>
.icon-bluesky {
  display: inline-block;
  width: 48px;
  height: 48px;
  background-color: #0085ff;
  border-radius: 50%;
  margin: 2.5px;
  vertical-align: middle;
}

.icon-bluesky svg {
  width: 50%;
  height: 100%;
}
</style>
