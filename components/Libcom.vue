<template>
  <Card
    title="LibCom"
    :image="libcom_header"
  >
    <p class="card-text">
      積読管理アプリLibComです。本をバーコードから登録して、グラフを見ながら本の進捗を管理できます!
    </p>
    <a href="https://apps.apple.com/gb/app/libcom/id1455763687" target="_blank">
      <img src="~/static/ioc_icon.svg" decoding="async">
    </a>
    <h3>使用技術</h3>
    <div class="techs">
      <div>
        <img src="~/static/swift_logo.svg" decoding="async"/>
        <p>Swift</p>
      </div>
    </div>
  </Card>
</template>

<script>
  import Card from '~/components/Card.vue'
  import LibcomHeader from '~/static/libcom_header.webp'

  export default {
    name: "Libcom",
    components: {
      Card,
    },
    data() {
      return {
        libcom_header: LibcomHeader,
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