<template>
<div>
  Hello World!
  {{$store.state.messages}}
  <button @click="RECEIVE_MESSAGE('first')">first</button>
</div>
</template>

<script>
import { mapMutations } from 'vuex'

export default {
  methods: {
    ...mapMutations({
      RECEIVE_MESSAGE: 'RECEIVE_MESSAGE'
    })
  }
}
</script>

<style>
body {
  font-size: 5vh;
}
</style>