<template>
  <div class="reveal">
    <div class="slides">
      <page-cover></page-cover>
      <page-kuro></page-kuro>
      <page-qna></page-qna>
    </div>
  </div>
</template>

<script lang="coffee" type="text/coffeescript">
Reveal = require "reveal.js"
module.exports =
  components:
    "page-cover": require './components/Cover.vue'
    "page-kuro": require './components/Kuro.vue'
    "page-qna": require './components/QnA.vue'
  ready: () ->
    Reveal.initialize()
    return
</script>
