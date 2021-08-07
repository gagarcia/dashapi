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
              <apexchart type="line" height="350" width="400" :options="chartOptions" :series="series"></apexchart>
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
      series: [{
        name: 'Desktops',
        data: [10, 41, 35, 51, 49, 62, 69, 91, 148]
      }],
      responsive: [{
        breakpoint: 480,
        options: {
          chart: {
            width: 370
          },
          legend: {
            position: 'bottom'
          }
        }
      }],
      chartOptions: {
        chart: {
          height: 350,
          type: 'line',
          zoom: {
            enabled: false
          }
        },
        dataLabels: {
          enabled: false
        },
        stroke: {
          curve: 'straight'
        },
        title: {
          align: 'left'
        },
        grid: {
          row: {
            colors: ['#f3f3f3', 'transparent'], // takes an array which will be repeated on columns
            opacity: 0.5
          }
        },
        xaxis: {
          categories: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep']
        }
      }

    }
  }
}
</script>
