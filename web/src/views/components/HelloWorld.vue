<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2 @click="test">Ecosystem</h2>
    <lw-test />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Component from 'vue-class-component'

import Test from './text.vue'

@Component({
  name: 'sidebar',
  components: {
    'lw-test': Test
  }
})
export default class Sidebar extends Vue {
  msg:String = 'Welcome to my Vue.js App' 

  test() {
    // console.log('yes')
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/css/index';
.hello {
  color: blue;
}
</style>
