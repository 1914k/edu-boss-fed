<template>
  <div id="app">
    <h1>APP</h1>
    <div>{{a}}</div>
    <button class="test" @click="test">测试</button>
    <router-view />
  </div>
</template>

<script lang="ts">
// optionsAPI 写法
import Vue from 'vue'

export default Vue.extend({
  data () {
    return {
      a: 1,
      b: '2',
      c: [],
      d: {
        a: 1,
        b: '2'
      }
    }
  },
  methods: {
    test () {
      this.a.toString()
    }
  }
})
// classAPIs 写法
// import Vue from 'vue'
// import Component from 'vue-class-component'
// @Component
// export default class App extends Vue {
//   a = 1
//   b = '2'
//   c = []
//   d = {
//     a: 1,
//     b: '2'
//   }

//   test ():void {
//     console.log(this.a)
//   }
// }
</script>

<style lang="scss">
// @import '~@/styles/variables.scss';

.test {
  color: $warning-color;
}
</style>
