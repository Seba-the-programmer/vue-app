<template>
  <div>
    <button @click="this.$emit('clicked')">Click me</button>
  </div>
</template>

<script>

export default {
  name: 'Btn',
  
}
</script>