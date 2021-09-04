<script>
import { Bar } from "vue-chartjs";
export default {
  extends: Bar,
  props: {
    chartdata: {
      type: Object,
      default: null,
    },
    options: {
      type: Object,
      default: null,
    },
  },
  // data: () => ({
  //   chartdata: {
  //     labels: [
  //       "January",
  //       "February",
  //       "March",
  //       "April",
  //       "May",
  //       "June",
  //       "July",
  //       "August",
  //       "September",
  //       "October",
  //       "November",
  //       "December",
  //     ],
  //     datasets: [
  //       {
  //         label: "GitHub Commits",
  //         backgroundColor: "#f87979",
  //         data: [40, 20, 12, 39, 10, 40, 39, 80, 40, 20, 12, 11],
  //       },
  //     ],
  //   },
  //   options: {
  //     responsive: true,
  //     maintainAspectRatio: false,
  //   },
  // }),

  mounted() {
    // Overwriting base render method with actual data.
    this.renderChart(this.chartdata, this.options);
  },
};
</script>

<style lang="postcss" scoped>
</style>