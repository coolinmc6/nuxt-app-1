<script>
import { defineComponent } from '@vue/composition-api'

export default defineComponent({
  props: {
    text: {
      type: String,
      required: true
    },
    handler: {
      type: Function,
      required: true,
    },
  },
  setup() {},
})
</script>
<template>
  <button @click="handler">{{ text }}</button>
</template>
