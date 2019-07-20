<template>
  <div id="apps">
    <h2 class="subtitle">App</h2>
    <v-container grid-list-md text-xs-center>
      <v-layout row wrap>
        <Charto />
        <Markpark />
      </v-layout>
      <v-layout row wrap>
        <ChartoWeb />
        <Libcom />
      </v-layout>
    </v-container>
  </div>
</template>

<script>
  import LibcomHeader from '~/static/libcom_header.webp'
  import Charto from "./Charto";
  import ChartoWeb from "./ChartoWeb";
  import Markpark from "./Markpark";
  import Libcom from "./Libcom";

  export default {
    name: "Apps.vue",
    components: {
      Libcom,
      Markpark,
      ChartoWeb,
      Charto,
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