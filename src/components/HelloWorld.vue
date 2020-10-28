<template>
  <h1>{{ msg }}</h1>
  <button @click="count++">count is: {{ count }}</button>
  <p>
    Edit <code>components/HelloWorld.vue</code> to test hot module replacement.
  </p>
</template>

<script lang="ts">
  import { defineComponent } from 'vue'
  export default defineComponent({
    name: 'HelloWorld',
    props: {
      msg: { type: String, default: '' },
    },
    data: (): { count: number } => {
      return {
        count: 0,
      }
    },
  })
</script>
