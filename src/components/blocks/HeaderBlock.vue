<template>
    <header class="header">
        <!-- <img :src="require('../../assets/Logo.svg')" alt="image"> -->
        <Icon file_name="Logo.svg"></Icon>
        <p class="header__phone">+7 987 654 32-10</p>

    </header>
</template>

<script>
import Icon from '@/components/icons/Icon.vue'

export default {
  name: 'HeaderBlock',
  components: {
    Icon

  },
  props: {
    name: {
      type: String,
      default: ''
    }
  }
}
</script>

<style scoped lang="scss">
    .header{
        display: flex;
        flex-wrap: wrap;
        height: 34px;
        justify-content: space-between;
        align-items: center;
        background: #3278FF;
        padding: 13px 70px

    }
    .header__phone {
        color: #FFF;
        font-family: Roboto;
        font-size: 22px;
        font-style: normal;
        font-weight: 700;
        line-height: normal;
        margin: 0;
        padding:0;
    }

</style>
