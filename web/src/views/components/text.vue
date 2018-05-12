<style lang="scss" scoped>
h1 {
  color: red;
}
</style>

<template>
<h1>{{a}}</h1>
</template>

<script lang="ts">
import Vue from 'vue'
import Component from 'vue-class-component'
import { Prop } from 'vue-property-decorator'

@Component({
  components: {
  }
})

export default class App extends Vue {
  @Prop({default: 100})
  a:Number
  created () {
  }
  mounted () {
  }
  destroyed () {
  }
}
</script>
