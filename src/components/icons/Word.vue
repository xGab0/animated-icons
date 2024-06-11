<script setup>
</script>

<template>
    <svg id="word" class="cool" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 1200 1200" shape-rendering="geometricPrecision" text-rendering="geometricPrecision">
      <g id="word-u-card" transform="translate(-809.9104 17)" rx="80" ry="80">
        <rect id="word-s-rect1" class="jesus" width="650" height="200" rx="0" ry="0" transform="translate(1034.410353 215)" fill="#41a5ee"/>
        <rect id="word-s-rect2" width="650" height="200" rx="0" ry="0" transform="translate(1034.410353 215)" fill="#2b7cd3"/>
        <rect id="word-s-rect3" width="650" height="200" rx="0" ry="0" transform="translate(1034.410353 415)" fill="#185abd"/>
        <rect id="word-s-rect4" width="650" height="200" rx="0" ry="0" transform="translate(1034.410353 614)" fill="#103f91"/>
      </g>
      <g transform="translate(-.5 207)">
        <svg id="word-u-brand" width="450" height="450" style="border-radius: 34px;">
          <rect width="450" height="450" rx="0" ry="0" fill="#185abd" stroke-width="0"/>
          <text x="50%" y="60%" dominant-baseline="middle" text-anchor="middle" font-size="400" font-weight="bolder" fill="white">W</text>
        </svg>
      </g>
    </svg>
    <!--img src="@/assets/svg/word.svg" alt="My Happy SVG" width="300" height="300" class="cool"/-->
</template>

<style scoped>
svg {
  fill: yellow;
  display: inline-block;
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
#word-u-brand {
  filter: drop-shadow(8px 15px 8px rgba(38, 51, 115, 0.4));
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