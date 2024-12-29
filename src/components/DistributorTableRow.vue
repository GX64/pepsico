<script setup>
defineProps({
  company: {
    type: String,
    required: true,
  },
  last_month: {
    type: Number,
    required: true,
  },
  forecast: {
    type: Number,
    required: true,
  },
  avg: {
    type: Number,
    required: true,
  },

})
</script>

<template>
  <tr>
    <td class="company">{{ company }}</td>
    <td>{{ last_month }}</td>
    <td>{{ forecast }}</td>
    <td>{{ avg }}</td>
  </tr>
</template>

<style scoped>

td {
  border: 1px solid black;
  padding: 5px;
  text-align: left;
}
.company {
  font-weight:bold;
}
</style>
