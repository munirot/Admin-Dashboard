<script>
import { Bar } from "vue-chartjs";

export default {
  extends: Bar,
  mounted() {
    this.renderChart(
      {
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
          "December"
        ],
        datasets: [
          {
            label: "Aceleda",
            backgroundColor: "#f87979",
            data: [40, 20, 12, 39, 10, 40, 39, 80, 40, 20, 12, 11]
          },
          {
            label: "ABA",
            backgroundColor: "orange",
            data: [90, 50, 3, 43, 50, 20, 19, 32, 10, 9, 72, 11]
          }
        ]
      },
      { responsive: true, maintainAspectRatio: false }
    );
  }
};
</script>