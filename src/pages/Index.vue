<template>
    <q-page>
        <div class="container q-pa-sm">
          <div class="row justify-start">
            <p class="text-h4 text-brand">Cotações</p>
          </div>
          <div class="row justify-start">
            <div class="column">
              <div class="container"><CardLine /></div>
              <div><CotacoesPeriodo /></div>
            </div>
            <q-reponsive :ratio="16/9" class="col">
              <div class="container"><ListaApis /></div>
            </q-reponsive>
        </div>
      </div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'
// import Card from '../components/Card.vue'
// import CardPie from '../components/CardPie.vue'
// import CardDonut from '../components/CardDonut.vue'
import CardLine from '../components/CardLine.vue'
import CotacoesPeriodo from '../components/CotacoesPeriodo.vue'
import ListaApis from '../components/ListaApis.vue'

export default defineComponent({
  name: 'PageIndex',
  components: {
    // Card,
    // CardPie,
    // CardDonut,
    CardLine,
    CotacoesPeriodo,
    ListaApis
  }
})
</script>

<style scoped>
  .text-brand {
    color: #30c5ff;
  }
</style>
