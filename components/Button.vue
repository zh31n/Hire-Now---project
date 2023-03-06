<template>
    <button @click="$emit('click')"><slot></slot></button>
</template>

<script>
export default {
  components: {},
  props: {
  },
  data() {
    return {
      
    }
  },
}
</script>

<style scoped>

</style>