<template>
  <div>
    <Navbar />
    <h1>This is DASHBOARD</h1>
    <div id="chart_div">
      <GChart
        type="LineChart"
        :data="chartData"
        :options="chartOptions"
      />
    </div>
  </div>
</template>

<script>
import { GChart } from 'vue-google-charts'
import Navbar from '../components/Navbar.vue'

export default {
  name: 'Dashboard',

  components: {
    GChart,
    Navbar
  },

  data () {
    return {
      // Array will be automatically processed with visualization.arrayToDataTable function
      chartData: [
        ['Gün', 'Harcama', 'Expenses', 'Profit'],
        ['2014', 1000, 400, 200],
        ['2015', 1170, 460, 250],
        ['2016', 660, 1120, 300],
        ['2017', 1030, 540, 350]
      ],
      chartOptions: {
        chart: {
          title: 'Company Performance',
          subtitle: 'Sales, Expenses, and Profit: 2014-2017'
        }
      }
    }
  }
}
</script>
