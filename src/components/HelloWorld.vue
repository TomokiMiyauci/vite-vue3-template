<template>
  <h1>{{ msg }}</h1>
  <button @click="count++">count is: {{ count }}</button>
  <p>
    Edit <code>components/HelloWorld.vue</code> to test hot module replacement.
  </p>
</template>

<script lang="ts">
  export default {
    name: 'HelloWorld',
    props: {
      msg: { type: String, default: '' },
    },
    data: (): { count: number } => {
      return {
        count: 0,
      }
    },
  }
</script>
