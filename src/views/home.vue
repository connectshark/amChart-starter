<template>
  <main>
    <h1 class="title">第一頁由此開始</h1>
  </main>
</template>

<script>
export default {
  setup () {
    return {

    }
  }
}
</script>

<style lang="scss" scoped>
main {
  height: 100vh;
  background-color: #111111;
  display: grid;
  place-items: center;
  .title {
    color:  transparent;
    font-size: 4rem;
    background-clip: text;
    -webkit-background-clip: text;
    background-image: linear-gradient(to bottom, #5ee7df 0%, #b490ca 100%);
  }
}
</style>