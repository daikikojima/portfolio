<template>
  <div class="info-boxes">
    <CareerInfoBox/>
    <SkillInfoBox />
  </div>
</template>

<script>
  import SkillInfoBox from '~/components/SkillInfoBox.vue'
  import CareerInfoBox from '~/components/CareerInfoBox.vue'
  export default {
    name: "InfoBoxes",
    components: {
      CareerInfoBox,
      SkillInfoBox
    }
  }
</script>

<style lang="scss" scoped>
  ul{
    &.terminal-rst{
      padding: 0;
    }
    li {
      list-style: none;
      margin: 2% 0;
    }
  }
  .terminal-img {
    height: 100px;
  }
</style>