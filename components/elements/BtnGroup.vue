<template>
  <!-- <div class="btn-group border border-gray-300 inline-flex divide-x rounded">
    <btn2 variant="primary">Button 1</btn2>
    <btn2 variant="2">Button 2</btn2>
    <btn2 variant="2">Button 3</btn2>
  </div>-->
  <div
    ref="btnGroup"
    class="btn-group inline-flex"
    :class="[variant, shape, size, {'outlined': outlined}]"
  >
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: {
    variant: {
      type: String,
      default: "default",
    },
    size: {
      type: String,
      default: "", // mini, default, compact, large || xs, sm, default, md, lg
    },
    shape: {
      type: String,
      default: "",
    },
    disabled: {
      type: Boolean,
      default: false,
    },
    outlined: {
      type: Boolean,
      default: false,
    },
    activeClass: String,
  },
  mounted() {
    // console.log(this.$refs.btnGroup.getElementsByTagName("button"));
  },
};
</script>

<style lang="postcss" scoped>
.btn-group {
  & button {
    @apply rounded-none border-r-0;
    &:first-child {
      @apply rounded-tl rounded-bl;
    }
    &:last-child {
      @apply rounded-tr rounded-br border-r;
    }
  }
}
</style>