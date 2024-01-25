<template>
    <button class="button_ui">{{ name }}</button>
</template>

<script>

export default {
  name: 'ButtonUi',
  props: {
    name: {
      type: String,
      default: ''
    }

  }
}
</script>

<style scoped lang="scss">
.button_ui {
  cursor: pointer;
  border-radius: 7px;
  color:white;
  background: #3278FF;
  width:141px;
  font-family: Roboto;
  font-size: 20px;
  font-style: normal;
  font-weight: 500;
  border: none;
  padding: 6px;
}

</style>
