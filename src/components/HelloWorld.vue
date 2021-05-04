<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <button v-on:click="reverse">Reverse message</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  methods:{
    reverse()
    {
      this.msg = this.msg.split('').reverse().join('')
    }
  }
}
</script>

<style scoped>

</style>
