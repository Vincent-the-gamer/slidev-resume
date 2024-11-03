<script setup lang="ts">
import { replaceAllNotChinese } from '../utils'

const props = defineProps<{
  list: string[]
  listStyleType?: string
}>()

const lists = props.list.map(item => replaceAllNotChinese(item))

const classnames
  = (props.listStyleType || 'decimal')
  + (props.listStyleType !== 'none' ? ' pl-5' : '')
</script>

<template>
  <ul :class="classnames">
    <li v-for="(item, index) in lists" :key="index" v-html="item" />
  </ul>
</template>

<style scoped>
.slidev-layout ul,
.slidev-layout li {
  margin: 0;
  padding: 0;
}
.slidev-layout ul.pl-5 {
  padding-left: 2rem;
}
.slidev-layout ul {
  list-style-type: v-bind(listStyleType);
}
</style>
