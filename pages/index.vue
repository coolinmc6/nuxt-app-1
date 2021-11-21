<template>
  <div>Index.vue</div>
</template>
<script>
import { defineComponent } from '@vue/composition-api'

export default defineComponent({
  setup(_props, context) {
    console.log(context);
  },
})
</script>
