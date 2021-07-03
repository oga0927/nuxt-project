<template>
  <button class="button button-default">
    <p class="text">
      <slot>default</slot>
    </p>
  </button>
</template>

<script>
export default {
  
}
</script>

<style lang="scss" scoped>
  .button-default {
    background-color: $color-font-sub;
    padding: 8px 16px;
    border-radius: 8px;

    > .text {
      color: $color-font-sub;
    }
  }
</style>