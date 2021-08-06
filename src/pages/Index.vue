<template>
    <q-page>
      <div class="row justify-center">
      <div><CardPie /></div>
      <div><CardPie /></div>
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
import CardPie from './CardPie.vue'

export default defineComponent({
  name: 'PageIndex',
  components: {
    Card,
    CardPie
  }
})
</script>
