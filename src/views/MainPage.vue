<template>
    <div class="main">
        <HeaderBlock/>
        <MainBlock></MainBlock>
    </div>
</template>

<script>
import HeaderBlock from '@/components/blocks/HeaderBlock.vue'
import MainBlock from '@/components/blocks/MainBlock.vue'

export default {
  name: 'MainPage',
  components: {
    MainBlock,
    HeaderBlock
  },
  props: {
  }
}
</script>

<style scoped lang="scss">
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;700&family=Roboto:wght@400;500;700&display=swap');

  .main {
    margin: 0;
    min-width: 500px;
  }
</style>
