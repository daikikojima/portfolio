<template>
  <Card
    title="CharTo for Web"
    :image="charto_web_header"
  >
    <p class="card-text">タスク管理ツールCharToのWeb版です。PWAにも対応しております。
      ChartとTodoを掛け合わせたものとなっております。
      <a target="_blank" href="https://charto-abc1d.firebaseapp.com/">こちら</a></p>
    <h3>使用技術</h3>
    <div class="techs">
      <div>
        <img src="~/static/vue.webp" decoding="async"/>
        <p>Vue.js</p>
      </div>
      <div>
        <img src="~/static/firebase_logo.webp" decoding="async"/>
        <p>Firebase</p>
      </div>
    </div>
  </Card>
</template>

<script>
  import Card from '~/components/Card.vue'
  import CharToWebHeader from '~/static/charto_web_header.webp'

  export default {
    name: "ChartoWeb",
    components: {
      Card,
    },
    data() {
      return {
        charto_web_header: CharToWebHeader,
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