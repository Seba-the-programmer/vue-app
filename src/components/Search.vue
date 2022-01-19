<template>
  <div>
    <input type="text" :value="value" @input="handleInput">
  </div>
</template>

<script>

export default {
  name: 'Search',
  props: {
    value: {
      type: String,
      required: true,
      default: 'Type anything'
    }
  },
  methods: {
    handleInput() {
      this.$emit('input')
    }
  }
}
</script>