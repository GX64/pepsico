<script setup lang="ts">
import DistributorTableRow from './DistributorTableRow.vue';

</script>

<template>
  <table>
    <tr>
    <th>Name</th>
    <th>Goods shipped last month</th>
    <th>Forecast for coming month</th>
    <th>Average</th>
  </tr>
    <DistributorTableRow company="Company 1" last_month=10000 forecast=11000 avg=9000 />
    <DistributorTableRow company="Company 2" last_month=20000 forecast=19000 avg=18000 />
    <DistributorTableRow company="Company 3" last_month=15000 forecast=16000 avg=17000 />
    <DistributorTableRow company="Company 4" last_month=7000 forecast=6000 avg=8000 />
  </table>
</template>


<style scoped>
table {
  border: 1px solid black;
  border-collapse: collapse;
}
th {
  border: 1px solid black;
  background-image: linear-gradient(to bottom, rgb(199, 199, 199), rgb(230, 230, 230));
  padding: 5px;
  text-align: left;
}
</style>
