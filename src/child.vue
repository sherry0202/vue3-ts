<template>

  <input :value="msg" @input="(e)=>$emit('update:msg', e.data)"/>
</template>

<script>
export default {
  name: "child",
  props: ['msg'],
  data() {
    return {
      a: '111'
    }
  },
  methods: {

  }
}
</script>

<style scoped>

</style>