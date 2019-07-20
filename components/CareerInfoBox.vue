<template>
  <terminal-box functional>
    <p>$ show Career</p>
    <ul class="terminal-rst">
      <li>2014.4 ~ 2018.3: Kyoto Univ, Fac of Engineering, Dept of Informatics</li>
      <li>2017.4 ~ 2018.3: Studied @ Information System Group</li>
      <li>2019.4 ~ Now: Kyoto Univ, Grad School of Informatics, Dept of System Science</li>
      <li>2019.4 ~ Now: Studying @ Nakashima lab (Applied Informatics Group)</li>
    </ul>
  </terminal-box>
</template>

<script>
  import TerminalBox from '~/components/TerminalBox.vue'

  export default {
    name: "CareerInfoBox",
    components: {
      TerminalBox
    }
  }
</script>

<style scoped>

</style>