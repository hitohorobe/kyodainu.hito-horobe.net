<script>
export default {
  name: 'IconX',
  setup() {
    const text = '巨大な犬、巨犬（きょだいぬ）'
    const siteUrl = 'https://kyodainu.hito-horobe.net/'
    const url = 'https://twitter.com/intent/tweet?text=' + encodeURIComponent(text + '\n' + siteUrl)
    return { url }
  },
}
</script>

<template>
  <div class="icon-x">
    <a v-bind:href="url" target="_blank">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        x="0px"
        y="0px"
        width="16"
        height="16"
        viewBox="0,0,256,256"
        style="vertical-align: sub"
      >
        <g
          fill-opacity="0"
          fill="#ffffff"
          fill-rule="nonzero"
          stroke="none"
          stroke-width="1"
          stroke-linecap="butt"
          stroke-linejoin="miter"
          stroke-miterlimit="10"
          stroke-dasharray=""
          stroke-dashoffset="0"
          font-family="none"
          font-weight="none"
          font-size="none"
          text-anchor="none"
          style="mix-blend-mode: normal"
        >
          <path d="M0,256v-256h256v256z" id="bgRectangle"></path>
        </g>
        <g
          fill="#ffffff"
          fill-rule="nonzero"
          stroke="none"
          stroke-width="1"
          stroke-linecap="butt"
          stroke-linejoin="miter"
          stroke-miterlimit="10"
          stroke-dasharray=""
          stroke-dashoffset="0"
          font-family="none"
          font-weight="none"
          font-size="none"
          text-anchor="none"
          style="mix-blend-mode: normal"
        >
          <g transform="scale(5.12,5.12)">
            <path
              d="M5.91992,6l14.66211,21.375l-14.35156,16.625h3.17969l12.57617,-14.57812l10,14.57813h12.01367l-15.31836,-22.33008l13.51758,-15.66992h-3.16992l-11.75391,13.61719l-9.3418,-13.61719zM9.7168,8h7.16406l23.32227,34h-7.16406z"
            ></path>
          </g>
        </g>
      </svg>
    </a>
  </div>
</template>

<style scoped>
.icon-x {
  display: inline-block;
  width: 48px;
  height: 48px;
  background-color: #000;
  border-radius: 50%;
  margin: 2.5px;
  vertical-align: middle;
}

.icon-x svg {
  width: 50%;
  height: 100%;
}
</style>
