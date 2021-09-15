<template>
  <Layout class="grid md:grid-cols-12 gap-2">
    <VerticalNav class="w-full col-span-2">
      <VerticalNavSection title="Reports">
        <VerticalNavItem to="/page">Geofence Report</VerticalNavItem>
        <VerticalNavItem>Asset Dwell Report</VerticalNavItem>
        <VerticalNavItem>TIR Report</VerticalNavItem>
        <VerticalNavItem>Fill Report</VerticalNavItem>
        <VerticalNavItem>Discharge Report</VerticalNavItem>
        <VerticalNavItem>Refill Report</VerticalNavItem>
        <VerticalNavItem>Command Report</VerticalNavItem>
        <VerticalNavItem>Decoded Messages</VerticalNavItem>
        <VerticalNavItem>Raw Messages</VerticalNavItem>
      </VerticalNavSection>
    </VerticalNav>
    <div class="col-span-10 grid grid-cols-2 gap-2 pr-4 py-2">
      <Card class="p-3">
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
      </Card>
      <Card class="p-3">
        <h5>Bar Chart</h5>
        <BarChart :chart-data="chartData" :options="chartOptions" class="relative"></BarChart>
      </Card>
      <Card class="p-3 text-right">
        <div class="flex justify-between">
          <h5>Line Chart</h5>
          <btn2 size="xs" shape="rounded" @click="fillData('line')">Randomize Data</btn2>
        </div>
        <LineChart :chart-data="lineChartData" :options="chartOptions" class="relative"></LineChart>
      </Card>
      <Card class="p-3 text-right">
        <div class="flex justify-between">
          <h5>Area Chart</h5>
          <btn2 size="xs" shape="rounded" @click="fillData('area',true)">Randomize Data</btn2>
        </div>
        <LineChart :chart-data="areaChartData" :options="chartOptions" class="relative"></LineChart>
      </Card>
      <Card class="p-3">
        <h5>Pie Chart</h5>
        <PieChart :chart-data="pieChartData" :options="chartOptions" class="relative"></PieChart>
      </Card>
      <Card class="p-3">
        <h5>Doughnut Chart</h5>
        <DoughNutChart :chart-data="pieChartData" :options="chartOptions" class="relative"></DoughNutChart>
      </Card>
      <Card class="p-3">
        <h5>Radar Chart</h5>
        <RadarChart :chart-data="radaraChartData" :options="chartOptions" class="relative"></RadarChart>
      </Card>
    </div>
  </Layout>
</template>

<script>
import resolveConfig from "tailwindcss/resolveConfig";
import tailwindConfig from "~/tailwind.config.js";
import {
  Btn2,
  Layout,
  BarChart,
  LineChart,
  PieChart,
  RadarChart,
  DoughNutChart,
  Card,
  Badge,
  Status,
  Heading,
  Dropdown,
  DropdownItem,
  Avatar,
  VerticalNav,
  VerticalNavSection,
  VerticalNavItem,
} from "@tkweb/elements";
const fullConfig = resolveConfig(tailwindConfig);
const colors = fullConfig.theme.colors;
const primaryColor = fullConfig.theme.colors.primary;
const greenColor = fullConfig.theme.colors.emerald;
export default {
  components: {
    Btn2,
    Layout,
    BarChart,
    Dropdown,
    Badge,
    Status,
    DropdownItem,
    LineChart,
    PieChart,
    DoughNutChart,
    RadarChart,
    Card,
    Heading,
    Avatar,
    VerticalNav,
    VerticalNavSection,
    VerticalNavItem,
  },
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
      pieChartData: {
        labels: ["Red", "Green", "Yellow"],
        datasets: [
          {
            label: "My First Dataset",
            data: [300, 50, 100, 100],
            backgroundColor: [
              colors.red[500],
              colors.green[600],
              colors.yellow[300],
              colors.gray[300],
            ],
            hoverOffset: 4,
          },
        ],
      },
      radaraChartData: {
        labels: [
          "Eating",
          "Drinking",
          "Sleeping",
          "Designing",
          "Coding",
          "Cycling",
          "Running",
        ],
        datasets: [
          {
            label: "My First Dataset",
            data: [65, 59, 90, 81, 56, 55, 40],
            fill: true,
            backgroundColor: "rgba(255, 99, 132, 0.2)",
            borderColor: "rgb(255, 99, 132)",
            pointBackgroundColor: "rgb(255, 99, 132)",
            pointBorderColor: "#fff",
            pointHoverBackgroundColor: "#fff",
            pointHoverBorderColor: "rgb(255, 99, 132)",
          },
          {
            label: "My Second Dataset",
            data: [28, 48, 40, 19, 96, 27, 100],
            fill: true,
            backgroundColor: "rgba(54, 162, 235, 0.2)",
            borderColor: "rgb(54, 162, 235)",
            pointBackgroundColor: "rgb(54, 162, 235)",
            pointBorderColor: "#fff",
            pointHoverBackgroundColor: "#fff",
            pointHoverBorderColor: "rgb(54, 162, 235)",
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