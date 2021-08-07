<template>
    <q-page>
      <div class="container q-pa-md">
        <div class="row justify-start">
          <p class="text-h6 h6">Cotações</p>
        </div>
        <div class="row justify-center">
          <div><CardPie /></div>
          <div><CardDonut /></div>
          <div><CardDonut /></div>
          <div><CardLine /></div>
          <div><Card /></div>
          <div><Card /></div>
          <div><Card /></div>
          <div><Card /></div>
          <div><Card /></div>
          <div><Card /></div>
          <div><Card /></div>
      </div>
      </div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'
import Card from './Card.vue'
import CardPie from './CardPie.vue'
import CardDonut from './CardDonut.vue'
import CardLine from './CardLine.vue'

export default defineComponent({
  name: 'PageIndex',
  components: {
    Card,
    CardPie,
    CardDonut,
    CardLine
  }
})
</script>
