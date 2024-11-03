<script setup lang="ts">
import { replaceAllNotChinese } from '../utils'

defineProps<{
  itemKey: string
  itemValue: string
}>()
</script>

<template>
  <div class="mb-1">
    <span v-if="itemKey">{{ itemKey }}: </span>
    <span v-html="replaceAllNotChinese(itemValue)" />
  </div>
</template>
