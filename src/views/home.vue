<template>
  <main>
    <h1 class="hello" ref="root">第一頁由此開始</h1>
  </main>
</template>

<script setup>
import { onMounted, ref } from 'vue'
import { useChart } from '../chart-core'
const root = ref(null)

const { createChart } = useChart()
onMounted(() => {
  createChart({ rootRef: root.value })
})
</script>

<style lang="scss" scoped>
main {
  height: 100vh;
  display: grid;
  place-items: center;
  .hello {
    width: 100%;
    height: 500px;
  }
}
</style>