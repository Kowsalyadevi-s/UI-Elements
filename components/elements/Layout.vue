<template>
  <div class="layout mx-auto w-full p-1">
    <slot>Layout Content</slot>
  </div>
</template>

<script>
export default {};
</script>

<style lang="postcss" scoped>
.layout {
  &.compact {
    @apply w-2/3;
  }
}
</style>