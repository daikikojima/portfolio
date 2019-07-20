<template>
  <Card
    title="CharTo"
    :image="charto_header"
  >
    <p class="card-text">タスク管理ツールCharToです。
      ChartとTodoを掛け合わせたものとなっております。</p>
    <a
      target="_blank"
      href='https://play.google.com/store/apps/details?id=com.jikoapps.charto&pcampaignid=MKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1'><img
      alt='Get it on Google Play'
      src='https://play.google.com/intl/en_us/badges/images/generic/en_badge_web_generic.png'
    /></a>
    <h3>使用技術</h3>
    <div class="techs">
      <div>
        <img src="~/static/kotlin_logo.webp"/>
        <p>Kotlin</p>
      </div>
      <div>
        <img src="~/static/firebase_logo.webp"/>
        <p>Firebase</p>
      </div>
    </div>
  </Card>
</template>

<script>
  import Card from '~/components/Card.vue'
  import CharToHeader from '~/static/charto_header.webp'

  export default {
    name: "Charto",
    components: {
      Card,
    },
    data() {
      return {
        charto_header: CharToHeader,
      }
    }
  }
</script>

<style lang="scss" scoped>
  img {
    height: 100px;
  }

  .techs {
    display: flex;
    justify-content: space-around;

    > img {
      height: 150px;
    }
  }

  .card-text {
    text-align: left;
  }
</style>