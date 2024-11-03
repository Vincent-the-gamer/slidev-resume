<script setup lang="ts">
interface Experience {
  time: string[]
  company: string
  role: string
}

defineProps<{
  title: string
  experiences: Experience[]
}>()
</script>

<template>
  <div mt-6>
    <h2 text-l mb-2 font-bold>
      {{ title }}
    </h2>
    <div>
      <div w-full flex flex-col mb-1>
        <div v-for="(item, index) in experiences" :key="index" py-1 my-0>
          <span v-if="/[0-9\.]/.test(item.time[1])" mr-5 hack>
            {{ item.time[0] }} ~ {{ item.time[1] }}
          </span>
          <span v-else class="hack" mr-5>
            {{ item.time[0] }} ~
            <span mr-10 song>{{ item.time[1] }}</span>
          </span>
          <span mr-15>{{ item.company }}</span>
          <span mr-15>{{ item.role }}</span>
        </div>
      </div>
    </div>
  </div>
</template>
