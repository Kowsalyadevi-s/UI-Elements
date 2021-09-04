<template>
  <Layout class="compact grid md:grid-cols-2 gap-2">
    <card class="p-3">
      <div class="space-y-4">
        <div class="space-y-4">
          <h3>Kodaikanal</h3>
          <p>Kodaikana Wellness Spa: India's No. 1 Family Spa Chain with national presence across top cities: Hotel Spa Operator, Villa Day Spas offering Reflexology, Full Body Massages, Facials, Scrubs, Wraps & use handmade, pure, chemical-free products. Best spa in Hyderabad, Ahmedabad,</p>
        </div>
        <div>
          Suggested duration
          <p class="font-bold">1-2 hours</p>
        </div>
        <div>
          Suggest edits to improve what we show.
          <a class="link">Improve this listing</a>
        </div>
        <btn2 shape="rounded" class="w-full" variant="dark">
          <div class="w-full">See more options</div>
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor">
            <path
              fill-rule="evenodd"
              d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z"
              clip-rule="evenodd"
            />
          </svg>
        </btn2>
      </div>
    </card>
    <card class="p-3">
      <BarChart :chartdata="chartData" :options="chartOptions" class="relative"></BarChart>
    </card>
    <card class="p-3 text-right">
      <btn2 size="xs" shape="rounded" @click="fillData('line')">Randomize Data</btn2>
      <LineChart :chart-data="lineChartData" :options="chartOptions" class="relative"></LineChart>
    </card>
    <card class="p-3 text-right">
      <btn2 size="xs" shape="rounded" @click="fillData('area',true)">Randomize Data</btn2>
      <LineChart :chart-data="areaChartData" :options="chartOptions" class="relative"></LineChart>
    </card>
  </Layout>
</template>

<script>
import resolveConfig from "tailwindcss/resolveConfig";
import tailwindConfig from "~/tailwind.config.js";
const fullConfig = resolveConfig(tailwindConfig);

const primaryColor = fullConfig.theme.colors.primary;
const greenColor = fullConfig.theme.colors.emerald;
export default {
  data() {
    return {
      lineChartData: null,
      areaChartData: null,
      chartData: {
        labels: [
          "January",
          "February",
          "March",
          "April",
          "May",
          "June",
          "July",
          "August",
          "September",
          "October",
          "November",
          "December",
        ],
        datasets: [
          {
            label: "Bookings",
            backgroundColor: greenColor[500],
            data: [40, 20, 12, 39, 10, 40, 39, 80, 40, 20, 12, 11],
          },
        ],
      },
      chartOptions: {
        responsive: true,
        maintainAspectRatio: false,
      },
    };
  },
  mounted() {
    this.fillData("line");
    this.fillData("area", true);
  },
  methods: {
    fillData(chart, bgColor) {
      const data = {
        labels: [
          this.getRandomInt(),
          this.getRandomInt(),
          this.getRandomInt(),
          this.getRandomInt(),
          this.getRandomInt(),
          this.getRandomInt(),
          this.getRandomInt(),
          this.getRandomInt(),
        ],
        datasets: [
          {
            label: "Data 1",
            borderColor: primaryColor[600],
            backgroundColor: bgColor ? primaryColor[500] : "transparent",
            data: [
              this.getRandomInt(),
              this.getRandomInt(),
              this.getRandomInt(),
              this.getRandomInt(),
              this.getRandomInt(),
              this.getRandomInt(),
              this.getRandomInt(),
              this.getRandomInt(),
            ],
            tension: 0.1,
          },
          // {
          //   label: "Data 2",
          //   borderColor: primaryColor[600],
          //   backgroundColor: bgColor ? primaryColor[600] : "transparent",
          //   data: [
          //     this.getRandomInt(),
          //     this.getRandomInt(),
          //     this.getRandomInt(),
          //     this.getRandomInt(),
          //     this.getRandomInt(),
          //     this.getRandomInt(),
          //     this.getRandomInt(),
          //     this.getRandomInt(),
          //   ],
          //   tension: 0.1,
          // },
          // {
          //   label: "Data 3",
          //   borderColor: primaryColor[800],
          //   backgroundColor: bgColor ? primaryColor[800] : "transparent",
          //   data: [
          //     this.getRandomInt(),
          //     this.getRandomInt(),
          //     this.getRandomInt(),
          //     this.getRandomInt(),
          //     this.getRandomInt(),
          //     this.getRandomInt(),
          //     this.getRandomInt(),
          //     this.getRandomInt(),
          //   ],
          //   tension: 0.1,
          // },
        ],
      };
      if (chart === "line") {
        this.lineChartData = data;
      } else {
        this.areaChartData = data;
      }
    },
    getRandomInt() {
      return Math.floor(Math.random() * (50 - 5 + 1)) + 5;
    },
  },
};
</script>

<style lang="postcss" scoped>
</style>