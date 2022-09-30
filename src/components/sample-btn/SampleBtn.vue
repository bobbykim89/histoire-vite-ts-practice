<script lang="ts" setup>
import type { Something, Color } from './types'

const miau: Something = {
  name: 'Manguito',
  isBird: true,
}
const someColor: Color = 'red'
console.log('this is a button', miau, someColor)
</script>

<template>
  <button class="px-4 py-2 bg-yellow-400">
    <slot></slot>
  </button>
</template>

<style lang="scss" scoped></style>
