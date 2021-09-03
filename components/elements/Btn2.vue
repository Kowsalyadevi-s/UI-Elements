<template>
  <button
    :bind="$attrs"
    v-on="$listeners"
    :disabled="disabled"
    :class="[variant, size, shape, {'outlined': outlined}]"
  >
    <slot>Button</slot>
  </button>
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
    rounded: {
      type: Boolean,
      default: false,
    },
    square: {
      type: Boolean,
      default: false,
    },
  },
};
</script>

<style lang="postcss" scoped>
/* Variants */
button {
  @apply place-items-center leading-5 text-center;

  & svg {
    @apply inline-flex place-items-center h-5 w-5;
  }

  &.xs {
    @apply px-2.5 py-1.5 text-xs leading-4;
    & svg {
      @apply h-4 w-4;
    }
  }
  &.sm {
    @apply px-3 py-2 text-sm leading-4;
    & svg {
      @apply h-4 w-4;
    }
  }
  &.lg {
    @apply px-4 py-2 text-base leading-6 rounded-md;
  }
  &.xl {
    @apply px-6 py-3 text-base leading-6 rounded-md;
  }

  &:disabled {
    @apply opacity-50;
  }
  &.default {
    @apply bg-white border border-gray-300 hover:bg-gray-50 hover:border-gray-400 hover:text-gray-900  focus:ring-2 focus:ring-gray-500 focus:ring-offset-gray-200;
  }

  &.primary {
    @apply bg-primary-600 border-primary-700 text-white hover:bg-primary-700 hover:border-primary-800 hover:text-white  focus:ring-2 focus:ring-primary-500 focus:ring-offset-primary-200;
  }

  &.dark {
    @apply bg-gray-900 border-black text-white hover:bg-gray-700 hover:border-gray-900 hover:text-white  focus:ring-2 focus:ring-gray-500 focus:ring-offset-gray-200;
  }

  &.positive {
    @apply bg-positive-600 border-positive-700 text-white hover:bg-positive-700 hover:border-positive-800 hover:text-white  focus:ring-2 focus:ring-positive-500 focus:ring-offset-positive-200;
  }

  &.negative {
    @apply bg-negative-600 border-negative-700 text-white hover:bg-negative-700 hover:border-negative-800 hover:text-white  focus:ring-2 focus:ring-negative-500 focus:ring-offset-negative-200;
  }

  &.rounded {
    @apply rounded-full;
  }
  &.square {
    @apply rounded-none;
  }

  &.outlined {
    @apply bg-transparent text-gray-800;
  }
}
</style>