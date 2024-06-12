<script setup>
</script>

<template>
    <svg id="word" class="big"
    xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
    viewBox="0 0 100 100"
    shape-rendering="geometricPrecision" text-rendering="geometricPrecision"
    >
      <symbol id="word-paper-rect-symbol" width="80" height="25">
        <rect id="word-paper-rect" width="100%" height="100%"/>
      </symbol>

      <!-- Everything under a white pixel will be visible -->
      <!-- Everything under a black pixel will be invisible -->
      <!--g>
        <svg id="word-u-card">
          <use href="#word-paper-rect-symbol" x="20" y="0" fill="#41a5ee" />
          <use href="#word-paper-rect-symbol" x="20" y="25" fill="#2b7cd3" />
          <use href="#word-paper-rect-symbol" x="20" y="50" fill="#185abd" />
          <use href="#word-paper-rect-symbol" x="20" y="75" fill="#103f91" />
        </svg>
      </g-->
      <g>
        <svg id="word-u-card">
          <use href="#word-paper-rect-symbol" x="20" y="0" fill="#41a5ee" />
          <use href="#word-paper-rect-symbol" x="20" y="25" fill="#2b7cd3" />
          <use href="#word-paper-rect-symbol" x="20" y="50" fill="#185abd" />
          <use href="#word-paper-rect-symbol" x="20" y="75" fill="#103f91" />
        </svg>
      </g>
      <g>
        <svg id="word-u-brand" width="40" height="40" x="0" y="30%">
          <rect width="100%" height="100%" ry="4" fill="#185abd"/>
          <text x="50%" y="58%" dominant-baseline="middle" text-anchor="middle" font-size="33" font-weight="bolder" fill="white">W</text>
        </svg>
      </g>
    </svg>
    <img src="@/assets/svg/word.svg" alt="My Happy SVG" width="300" height="300" class="cool">
</template>

<style scoped>
#word {
  overflow: visible;
}
#word-paper-rect-symbol {
  overflow: visible;
}
#word-u-card {
  overflow: visible;
}
#word-paper-rect {
  pointer-events: all;
  transition: all .1s ease-in-out;
}
#word-paper-rect:hover {
  transform-origin: 50% 50%; /* anything other than `0 0` to see the effect */
  transform-box: fill-box;

  /*animation: scaleheight 1s ease-in-out infinite alternate;*/
  /*animation: breathePaperCut .3s ease-in-out forwards;*/

  transform: scale3d(1.05, 1.05, 1);
}

#word-u-brand {
  filter: drop-shadow(4px 5px 2px rgba(2, 28, 89, 0.579));
}

@keyframes breathePaperCut {
  to {
    transform: scale3d(1.05, 1, 1);
  }
}

svg {
  fill: yellow;

}

#word-u-card {
  outline: solid 50px rgba(96, 149, 255, 0);
  outline-offset: 15px;
}
/*
#word-u-card:hover {
  outline-color: red
}
*/


.paper-card .first {
  fill: #41a5ee;
}
.paper-card .second {
  fill: #2b7cd3;
}
.paper-card .third {
  fill: #185abd;
}
.paper-card .fourth {
  fill: #185abd;
}

.jesus:hover {
  pointer-events: all;

  transform-style: preserve-3d;
  transform: translate3d(0px, -26px, 0px);

  transition: .4s ease-in-out transform;
}

.cool {
  display: flex;
  flex-direction: column;
  width: 300px;
  height: 300px;

  transform:
    rotateX(51deg)
    rotateZ(43deg);
  transform-style: preserve-3d;
  border-radius: 32px;
  box-shadow:
    1px 1px 0 1px #f9f9fb,
    -1px 0 28px 0 rgba(34, 33, 81, 0.01),
    28px 28px 28px 0 rgba(34, 33, 81, 0.25);
  transition:
    .4s ease-in-out transform,
    .4s ease-in-out box-shadow;

  &:hover {
    transform:
      translate3d(0px, -16px, 0px)
      rotateX(51deg)
      rotateZ(43deg);
    box-shadow:
      1px 1px 0 1px #f9f9fb,
      -1px 0 28px 0 rgba(34, 33, 81, 0.01),
      54px 54px 28px -10px rgba(34, 33, 81, 0.15);
  }
}
</style>