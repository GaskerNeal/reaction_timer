<template>
  <p>Result is {{score}}ms</p>
  <div v-if="score<300">
    <p>You are so fast.</p>
  </div>
  <div v-else-if="score>300 && score<500">
    <p>You are normal.</p>
  </div>
  <div v-else>
    <p>You are too slow.</p>
  </div>
</template>

<script>
export default {
    props:['score'],
}
</script>

<style>
p {
    color: green;
}
</style>