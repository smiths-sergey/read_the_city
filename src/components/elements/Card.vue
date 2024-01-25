<template>
    <div class="card">
      <Icon :file_name="icon_file_name"></Icon>
      <p class="card__title">{{ title1 }}</p>
      <p class="card__title">{{ title2 }}</p>
      <p class="card__author">{{author}}</p>
      <ButtonCard
        name="Купить"
      />
    </div>
</template>

<script>
import ButtonCard from '@/components/ui/Button.vue'
import Icon from '@/components/icons/Icon.vue'
export default {
  name: 'CardElement',
  components: {
    ButtonCard,
    Icon
  },
  props: {
    icon_file_name: {
      type: String,
      default: ''
    },
    title1: {
      type: String,
      default: ''
    },
    title2: {
      type: String,
      default: ''
    },
    author: {
      type: String,
      default: ''
    }

  }
}
</script>

<style scoped lang="scss">
.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 330px;
  padding-top: 19px;
  padding-left: 15px;
  padding-right: 15px;
  padding-bottom: 24px;
  border-radius: 10px;
  box-shadow: 1px 1px 4px 0px rgba(0, 0, 0, 0.30);

}

p {
  margin: 0;
  padding: 0;
}

.card__title {
  text-align: center;
  font-family: Roboto;
  font-size: 24px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}

.card__author{
  font-family: Roboto;
  font-size: 20px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  margin-top: 14px;
  margin-bottom: 34px;
}
.card__preview {
  padding-bottom: 16px;
}
</style>
