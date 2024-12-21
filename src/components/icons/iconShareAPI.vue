<script>
export default {
  name: 'IconShareAPI',
  methods: {
    share() {
      if (navigator.share) {
        navigator.share({
          title: '巨大な犬、巨犬（きょだいぬ）',
          text: '巨大な犬、巨犬（きょだいぬ）',
          url: 'https://kyodainu.hito-horobe.net/',
        })
      } else {
        console.log('navigator.share is not supported')
      }
    },
  },
}
</script>

<template>
  <div class="icon-share">
    <a v-on:click="share">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 24 24"
        width="16"
        height="16"
        style="vertical-align: sub"
      >
        <path
          fill="#000000"
          d="M18 16.08C17.24 16.08 16.56 16.38 16.05 16.88L8.91 12.7C8.96 12.47 9 12.24 9 12C9 11.76 8.96 11.53 8.91 11.3L15.05 7.12C15.56 7.62 16.24 7.92 17 7.92C18.66 7.92 20 6.58 20 4.92C20 3.26 18.66 1.92 17 1.92C15.34 1.92 14 3.26 14 4.92C14 5.16 14.04 5.39 14.09 5.62L7.95 9.8C7.44 9.3 6.76 9 6 9C4.34 9 3 10.34 3 12C3 13.66 4.34 15 6 15C6.76 15 7.44 14.7 7.95 14.2L14.09 18.38C14.04 18.61 14 18.84 14 19.08C14 20.74 15.34 22.08 17 22.08C18.66 22.08 20 20.74 20 19.08C20 17.42 18.66 16.08 17 16.08Z"
        />
      </svg>
    </a>
  </div>
</template>

<style scoped>
.icon-share {
  display: inline-block;
  width: 48px;
  height: 48px;
  background-color: #f0f0f0;
  border-radius: 50%;
  margin: 2.5px;
  vertical-align: middle;
}

.icon-share svg {
  width: 50%;
  height: 100%;
}
</style>
