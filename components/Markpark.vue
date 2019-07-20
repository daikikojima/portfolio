<template>
  <Card
    title="MarkPark"
    :image="markpark_header"
  >
    <p class="card-text">自転車の駐輪場所を記録し、自転車探しを手助けするアプリです。</p>
    <a
      target="_blank"
      href='https://play.google.com/store/apps/details?id=com.jiko.bycicle&pcampaignid=MKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1'><img
      alt='Get it on Google Play'
      src='https://play.google.com/intl/en_us/badges/images/generic/en_badge_web_generic.png'/></a>
    <h3>使用技術</h3>
    <div class="techs">
      <div>
        <img src="~/static/kotlin_logo.webp" decoding="async"/>
        <p>Kotlin</p>
      </div>
      <div>
        <img src="~/static/map_icon.webp" decoding="async"/>
        <p>Maps sdk for Android</p>
      </div>
    </div>
  </Card>
</template>

<script>
  import Card from '~/components/Card.vue'
  import MarkparkHeader from '~/static/markpark_header.webp'

  export default {
    name: "Markpark",
    components: {
      Card,
    },
    data() {
      return {
        markpark_header: MarkparkHeader,
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