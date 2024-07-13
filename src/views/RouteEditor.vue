<template>
  <div>
    <h2>Route Editor</h2>
    <div class="flex">
      <main>
        <svg xmlns="http://www.w3.org/2000/svg">
          <svg
            viewBox="-80 -80 160 160"
            x="100"
            y="100"
            width="160"
            height="160"
          >
            <!---->
            <defs>
              <mask id="circle">
                <circle cx="0" cy="0" r="50.5" fill="white"></circle>
              </mask>
            </defs>

            <path
              fill="none"
              stroke="red"
              stroke-width="2"
              d="M0,0 v-50 a50,50 0 0,0 -50,50 z"
            />
            <path
              fill="none"
              stroke="red"
              stroke-width="2"
              d="M0,0 v-50 a50,50 0 0,0 -50,50 z"
            />

            <circle
              cx="0"
              cy="0"
              r="50"
              fill="transparent"
              stroke="#333"
            ></circle>

            <g transform="rotate(0)" mask="url(#circle)">
              <rect
                class="interactive-area"
                x="-50"
                y="-50"
                width="50"
                height="50"
                fill="transparent"
                stroke="#333"
              ></rect>
              <text
                x="-20"
                y="-20"
                dominant-baseline="middle"
                text-anchor="middle"
                transform-origin="-20 -20"
                transform="rotate(-45)"
              >
                1
              </text>

              <rect
                x="0"
                y="-50"
                width="50"
                height="50"
                fill="transparent"
                stroke="#333"
              ></rect>
              <text
                x="20"
                y="-20"
                dominant-baseline="middle"
                text-anchor="middle"
                transform-origin="20 -20"
                transform="rotate(-45)"
              >
                2
              </text>

              <rect
                x="-50"
                y="0"
                width="50"
                height="50"
                fill="transparent"
                stroke="#333"
              ></rect>
              <text
                x="-20"
                y="20"
                dominant-baseline="middle"
                text-anchor="middle"
                transform-origin="-20 20"
                transform="rotate(-45)"
              >
                4
              </text>

              <rect
                x="0"
                y="0"
                width="50"
                height="50"
                fill="transparent"
                stroke="#333"
              ></rect>
              <text
                x="20"
                y="20"
                dominant-baseline="middle"
                text-anchor="middle"
                transform-origin="20 20"
                transform="rotate(-45)"
              >
                3
              </text>
            </g>
          </svg>
        </svg>
      </main>
      <aside>This is aside</aside>
    </div>
  </div>
</template>

<style scoped>
.flex {
  display: flex;
}
.flex > * {
  flex: 1;
}

aside {
  flex: 0 1 30%;
}

svg {
  width: 100%;
  height: 100%;
  min-height: 600px;
  background: #f8f8f8;
}

.interactive-area {
  fill: "#f8f8f8";
}
</style>
