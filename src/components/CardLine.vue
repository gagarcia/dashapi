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
            <div id="chart">
              <apexchart type="area" :options="chartOptions" :series="series"></apexchart>
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
        data: [10.000, 15.543, 12.789, 13.690, 30.000, 20.000, 15.000, 25.000, 30.345]
      }],
      responsive: [{
        breakpoint: 400,
        options: {
          chart: {
            width: '100%'
          },
          legend: {
            position: 'bottom'
          }
        }
      }],
      chartOptions: {
        chart: {
          toolbar: {
            show: false
          },
          height: 300,
          width: '100%',
          type: 'area',
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
          show: false
          // row: {
          //   colors: ['#f3f3f3', 'transparent'], // takes an array which will be repeated on columns
          //   opacity: 0.5
          // }
        },
        xaxis: {
          labels: {
            show: false
          },
          show: false,
          categories: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep']
        },
        yaxis: {
          labels: {
            show: false
          },
          show: false
        }
      }

    }
  }
}
</script>
