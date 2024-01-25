<template>
    <img :src="require('@/assets/'+file_name)" alt="image" class="card__preview">
</template>

<script>

export default {
  name: 'IconUi',
  props: {
    file_name: {
      type: String,
      default: ''
    }
  }
}
</script>

<style scoped lang="scss">
</style>
