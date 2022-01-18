<template>
  <div>
    <input type="text" value="value" @change="handleInput">
  </div>
</template>

<script>

export default {
  name: 'Search',
  props: {
    value: String,
  },
  methods: {
    handleInput() {
      this.$emit()
    }
  }
}
</script>