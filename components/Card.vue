<template>
    <v-flex xs12 md6>
      <v-card class="card">
        <v-img
          height="300"
          :lazy-src="image"
          :src="image"
        ></v-img>

        <v-card-title primary-title>
          <div>
            <div class="headline">{{title}}</div>
          </div>
        </v-card-title>
        <v-card-actions>
          <v-spacer/>
          <v-btn icon @click="show = !show">
            <v-icon>{{ show ? 'keyboard_arrow_up' : 'keyboard_arrow_down' }}</v-icon>
          </v-btn>
        </v-card-actions>
        <v-slide-y-transition>
          <v-card-text v-show="show">
            <slot/>
          </v-card-text>
        </v-slide-y-transition>
      </v-card>
    </v-flex>
</template>

<script>
  export default {
    name: "Card",
    props: [
      'title',
      'image'
    ],
    data: () => ({
      show: false,
    }),
  }
</script>

<style lang="scss" scoped>
  .card {
    v-img {
      height: 300px;
    }
  }
</style>