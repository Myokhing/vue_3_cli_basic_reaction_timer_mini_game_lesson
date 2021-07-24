<template>
  <div>
      <p>Result is: {{score}} ms</p>
      <div v-if="score < 250">
          <p>You are too fast</p>

      </div>
      <div v-else-if="score > 250 && score">
          <p>you are normal</p>
      </div>
      <div v-else>
          <p>you are too slow! try again</p>
      </div>
  </div>
</template>

<script>
export default {
props: ['score'],
}
</script>

<style>

</style>