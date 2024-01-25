<template>
    <div class="main__block_wrapper">
    <main class="main__block">
        <Card
            icon_file_name="image1.jpg"
            title1="Skyrim. История создания "
            title2="великой игры"
            author="Франк Экстанази"
        >
        </Card>
        <Card
            icon_file_name="image2.jpg"
            title1="Поисковое продвижение "
            title2="сайтов"
            author="Сергей Анисимов"
        >
        </Card>
        <Card
            icon_file_name="image3.jpg"
            title1="Английский"
            title2="для дизайнеров"
            author="Татьяна Магарина"
        >
        </Card>
        <Card
            icon_file_name="image4.jpg"
            title1="Дизайн и цвет."
            title2="Практикум"
            author="Шон Адамс"
        >
        </Card>
    </main>
  </div>
</template>

<script>
import Card from '@/components/elements/Card.vue'
export default {
  name: 'MainBlock',
  components: {
    Card
  }
}
</script>

<style scoped lang="scss">
.main__block_wrapper{
  display: grid;
  place-items: center;
  height: calc(100vh - 60px);
}
.main__block{
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  padding: 26px;
  gap: 26px;
}

</style>
