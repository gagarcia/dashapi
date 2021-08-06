<template>
    <q-page>
      <div class="row justify-center">
      <div><Card /></div>
      <div><Card /></div>
      <div><Card /></div>
      <div><Card /></div>
      <div><Card /></div>
      <div><Card /></div>
      <div><Card /></div>
      <div><Card /></div>
      <div><Card /></div>
      <div><Card /></div>
      <div><Card /></div>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'
import Card from './Card.vue'

export default defineComponent({
  name: 'PageIndex',
  components: {
    Card
  }
})
</script>
