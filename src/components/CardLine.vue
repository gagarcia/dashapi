<template>
  <div class="container q-px-xm q-py-md items-start">
    <q-card class="my-card">
      <q-card-section>
        <div class="column justify-start">
          <div class="row justify-start">
            <p class="text-h6 h6">Cotações Gerais</p>
          </div>
          <div class="row justify-start">
            <p class="text-h4 h4">R$ 84,000.00</p>
          </div>
          <div class="row full-width">
            <LineChart />
          </div>
        </div>
      </q-card-section>
    </q-card>
  </div>
</template>

<script>
import LineChart from './LineChart.vue'

export default {
  components: {
    LineChart
  },
  data () {
  }
}
</script>
