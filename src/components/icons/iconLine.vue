<script>
export default {
  name: 'IconLine',
  setup() {
    const text = '巨大な犬、巨犬（きょだいぬ）'
    const siteUrl = 'https://kyodainu.hito-horobe.net/'
    const url =
      'https://social-plugins.line.me/lineit/share?url=' +
      encodeURIComponent(siteUrl) +
      '&text=' +
      encodeURIComponent(text)
    return { url }
  },
}
</script>

<template>
  <div class="icon-line">
    <a v-bind:href="url" target="_blank">
      <svg
        xmlns="http://www.w3.org/2000/svg"
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
          <g transform="scale(5.33333,5.33333)">
            <path
              d="M25.12,44.521c-2.114,1.162 -2.024,-0.549 -1.933,-1.076c0.054,-0.314 0.3,-1.787 0.3,-1.787c0.07,-0.534 0.144,-1.36 -0.067,-1.887c-0.235,-0.58 -1.166,-0.882 -1.85,-1.029c-10.09,-1.327 -17.559,-8.342 -17.559,-16.717c0,-9.342 9.42,-16.943 20.995,-16.943c11.575,0 20.994,7.601 20.994,16.943c0,10.492 -11.128,17.134 -20.88,22.496zM18.369,25.845c0,-0.56 -0.459,-1.015 -1.023,-1.015h-2.856v-6.678c0,-0.56 -0.459,-1.015 -1.023,-1.015c-0.565,0 -1.023,0.455 -1.023,1.015v7.694c0,0.561 0.459,1.016 1.023,1.016h3.879c0.564,0.001 1.023,-0.456 1.023,-1.017zM21.357,18.152c0,-0.56 -0.459,-1.015 -1.023,-1.015c-0.565,0 -1.023,0.455 -1.023,1.015v7.694c0,0.561 0.459,1.016 1.023,1.016c0.565,0 1.023,-0.456 1.023,-1.016zM30.697,18.152c0,-0.56 -0.459,-1.015 -1.023,-1.015c-0.565,0 -1.025,0.455 -1.025,1.015v4.761l-3.978,-5.369c-0.192,-0.254 -0.499,-0.406 -0.818,-0.406c-0.11,0 -0.219,0.016 -0.325,0.052c-0.419,0.139 -0.7,0.526 -0.7,0.963v7.694c0,0.561 0.46,1.016 1.025,1.016c0.566,0 1.025,-0.456 1.025,-1.016v-4.759l3.976,5.369c0.192,0.254 0.498,0.406 0.818,0.406c0.109,0 0.219,-0.018 0.325,-0.053c0.42,-0.137 0.7,-0.524 0.7,-0.963zM36.975,20.984h-2.856v-1.817h2.856c0.566,0 1.025,-0.455 1.025,-1.015c0,-0.56 -0.46,-1.015 -1.025,-1.015h-3.879c-0.565,0 -1.023,0.455 -1.023,1.015c0,0.001 0,0.001 0,0.003v3.842v0.001c0,0 0,0 0,0.001v3.845c0,0.561 0.46,1.016 1.023,1.016h3.879c0.565,0 1.025,-0.456 1.025,-1.016c0,-0.56 -0.46,-1.015 -1.025,-1.015h-2.856v-1.817h2.856c0.566,0 1.025,-0.455 1.025,-1.015c0,-0.561 -0.46,-1.016 -1.025,-1.016z"
            ></path>
          </g>
        </g>
      </svg>
    </a>
  </div>
</template>

<style scoped>
.icon-line {
  display: inline-block;
  width: 48px;
  height: 48px;
  background-color: #00c300;
  border-radius: 50%;
  margin: 2.5px;
  vertical-align: middle;
}

.icon-line svg {
  width: 50%;
  height: 100%;
}
</style>
