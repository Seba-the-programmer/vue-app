<template>
  <div>
    <Search :value="val" @input="handleInput"/>
    <div>{{val}}</div>
    <div>
      <Btn @clicked="this.count++"/>
      Count: {{count}}
    </div>
  </div>
</template>

<script>
import Search from '@/components/Search.vue'
import Btn from '@/components/Btn.vue'
export default {
  name: 'App',
  components: {
    Search,
    Btn
  },
  data () {
    return {
      val: 'Type anything',
      count: 0
    }
  },
  methods: {
    handleInput(e) {
      this.val = e.target.value
    },
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
