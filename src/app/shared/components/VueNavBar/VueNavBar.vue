<template>
  <div :class="$style.vueNavBar" ref="nav">
    <slot />
  </div>
</template>

<script lang="ts">
export default {
  name: 'VueNavBar',
};
</script>

<style lang="scss" module>
@import '~@/app/shared/design-system';

.vueNavBar {
  width: $nav-bar-width;
  min-height: $nav-bar-height;
  color: $nav-bar-color;
  padding: $nav-bar-padding;
  z-index: $nav-bar-index;
  position: fixed;
  top: 0;
  left: 0;
  background: $nav-bar-bg;
}
</style>
