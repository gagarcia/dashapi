<template>
    <div class="container" id="chart">
        <apexchart type="area" :options="chartOptions" :series="series"></apexchart>
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
        name: 'Cotações',
        data: [10.000, 15.543, 12.789, 13.690, 30.000, 20.000, 25.000, 25.000, 30.345]
      }],
      responsive: [{
        breakpoint: 400,
        options: {
          chart: {
            width: '100%'
            // height: '100%'
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
          curve: 'straight',
          width: 1
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
