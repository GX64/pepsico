<script setup>
import DistributorTable from './components/DistributorTable.vue';
import NavBar from './components/NavBar.vue';
</script>

<template>
  <div style="display: block;">
    <header>
      <NavBar />
    </header>

    <main>
      <p>This is a site I made for the Forage PepsiCo Advanced Software Engineering job simulation. This website is not affiliated with or endorsed by PepsiCo.</p>
      <h2>Distributor information</h2>
      <br>
      <DistributorTable />
    </main>
  </div>
  <img class="background_image" src="/src/assets/chips.jpg" alt="potato chips" width="500" />
</template>

<style scoped>
header {
  /*top: 0;
  left: 0;
  position: fixed;*/
  width: 100%;
  display: flex;
  align-items: center;
  /*for vertically center*/
  background-color: rgb(35, 67, 143);
  border-bottom: 2px solid black;
}

main {
  padding: 20px;
  background-color: white;
  border-bottom: 2px solid black;
}

.background_image {
  position: absolute;
  bottom: 0;
  right: 0;
  z-index: -999;
}
</style>
