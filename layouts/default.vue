<template>
  <nuxt />
</template>

<style lang="less">
@import '~assets/global.less';

a {
  color: @link-color;
  text-decoration: none;

  & svg path {
    fill: @link-color;
  }

  &:hover {
    text-decoration: underline;
  }
}

html,
body {
  font-family: monospace;
  font-size: 16px;
  line-height: 1.5;
  font-weight: 400;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  background: @body-bg-color;
  color: @main-color;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

@-ms-viewport {
  width: device-width;
}

.section-title {
  font-size: 1.25rem;
  font-weight: 700;
  text-transform: uppercase;
  padding-bottom: 1rem;
  margin-bottom: 1rem;
  position: relative;
  margin-bottom: 1rem;

  &:after {
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    width: 100%;
    height: 2px;
    background: @delimiter-color;
  }
}

.tags-list {
  list-style: none;
  padding-left: 0;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  margin: 0.5rem 0 0 0;

  &__elem {
    display: inline-block;
    padding: 0.25em 0.4em;
    margin: 0 0.3rem 0.3rem 0;
    font-size: 75%;
    font-weight: 700;
    line-height: 1;
    text-align: center;
    white-space: nowrap;
    vertical-align: baseline;
    border-radius: 0.25rem;
  }
}
</style>
