<template>
    <q-card class="my-card">
        <div class="row justify-between q-pa-sm no-wrap">
            <div class="column">
                <div class="text-h6">{{ titulo }}</div>
                <div class="text-subtitle1">{{ subtitulo }}</div>
            </div>
            <div class="column">
              <LineChart />
            </div>
            <div class="column justify-center">
                <div>
                    <p class="text-weight-bold">R${{ cotacoes }}</p>
                </div>
                <div><PctVar :variacao="variacao" /></div>
            </div>
        </div>
    </q-card>
</template>

<script>
import PctVar from './PctVar.vue'
import LineChart from './LineChart.vue'

export default {
  name: 'Api',
  props: {
    titulo: {
      type: String
    },
    subtitulo: {
      type: String
    },
    variacao: {
      type: String,
      default: '0,00'
    },
    cotacoes: {
      type: String
    }
  },
  components: {
    PctVar,
    LineChart
  },
  data () {
    return {
    }
  }
}
</script>
