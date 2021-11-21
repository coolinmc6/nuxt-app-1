<template>
  <div>
    <h1>Hey man, this is {{ name }}</h1>
    <NuxtLink to="/inspire">Inspire</NuxtLink>
    <Button text="Click this!" :handler="buttonHandler" />
  </div>
</template>
<script>
import { defineComponent } from '@vue/composition-api';

export default defineComponent({
  setup() {
    const name = 'Colin';
    const buttonHandler = () => {
      console.log('button clicked!')
    }

    return {
      name, buttonHandler
    }
  },
})
</script>
