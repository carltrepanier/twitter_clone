<template>
  <div class="p-3 hover:bg-gray-100 curser-pointer dark:hover:bg-dim-300 border-b" :class="wrapperClasses">
    <slot></slot>
  </div>
</template>

<script setup>
  const {twitterBorderColor, defaultTransition} = useTailwindConfig()
  const wrapperClasses = computed(() => `${twitterBorderColor} ${defaultTransition}`)
</script>