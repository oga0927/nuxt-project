<template>
  <button 
    :class="{ 'color-red': itemStatus === 'red'}"
    class="button button-default"
  >
    <p class="text">
      <slot>default</slot>
    </p>
  </button>
</template>

<script>
export default {
  props: {
    itemStatus: {
      type: String,
      required: false,
      
    }
  },
}
</script>

<style lang="scss" scoped>
  .button-default {
    background-color: $color-font-sub;
    padding: 8px 16px;
    border-radius: 8px;
    font-size: 12px;

    &.color-red {
      background-color: red;
    }

    > .text {
      color: $color-font-sub;
    }
  }
</style>