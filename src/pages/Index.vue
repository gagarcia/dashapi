<template>
    <q-page>
      <div class="container q-pa-md">
        <div class="row justify-start">
          <p class="text-h6 text-brand">Cotações</p>
        </div>
        <div class="row justify-center">
          <div><CardLine /></div>
          <div><CardDonut /></div>
          <div><CardDonut /></div>
          <div><CardLine /></div>
          <div><CardPie /></div>
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
import Card from '../components/Card.vue'
import CardPie from '../components/CardPie.vue'
import CardDonut from '../components/CardDonut.vue'
import CardLine from '../components/CardLine.vue'

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

<style scoped>
  .text-brand {
    color: #30c5ff;
  }
</style>
