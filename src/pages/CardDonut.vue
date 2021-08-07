<template>
  <div class="q-pa-md row items-start q-gutter-md">
    <q-card class="my-card">
      <q-card-section>
        <div class="column justify-start">
          <div class="row justify-start">
            <p class="text-h6 h6">Cotações Gerais</p>
          </div>
          <div class="row justify-start">
            <p class="text-h4 h4">R$ 84,000.00</p>
          </div>
          <div class="row">
            <div id="chart">
              <apexchart
                type="donut"
                width="380"
                :options="chartOptions"
                :series="series"
              >
              </apexchart>
            </div>
          </div>
        </div>
      </q-card-section>
    </q-card>
  </div>
</template>

<script>
import VueApexCharts from 'vue3-apexcharts'

export default {
  components: {
    apexchart: VueApexCharts
  },
  data () {
    return {
      series: [44, 55, 41, 17, 15],
      chartOptions: {
        chart: {
          type: 'donut'
        },
        responsive: [{
          breakpoint: 480,
          options: {
            chart: {
              width: 400
            },
            legend: {
              position: 'bottom'
            }
          }
        }]
      }

    }
  }
}
</script>
