<template>
  <terminal-box>
    <p>$ show Skill</p>
    <ul class="terminal-rst">
      <li>C/C++</li>
      <li>JavaScript/TypeScript (especially skillful)</li>
      <ul>
        <li>Node.js</li>
        <li>Vue.js (Vuex)</li>
        <li>React</li>
      </ul>
      <li>Java/Kotlin</li>
      <ul>
        <li>Android apps</li>
        <li>Spring boot (a little bit)</li>
      </ul>
      <li>Swift</li>
      <ul>
        <li>iOS App Develop</li>
      </ul>
      <li>Ruby</li>
      <ul>
        <li>Ruby on Rails</li>
      </ul>
      <li>Python</li>
      <ul>
        <li>Data visualization</li>
        <li>Web scraping</li>
        <li>Web (Django)</li>
      </ul>
    </ul>
  </terminal-box>
</template>

<script>
  import TerminalBox from '~/components/TerminalBox.vue'

  export default {
    name: "SkillInfoBox",
    components: {
      TerminalBox
    }
  }
</script>

<style scoped>

</style>