<script setup>
import Navbar from "./components/Navbar.vue";
import Sidebar from "./components/Sidebar.vue";
import MainContent from "./components/MainContent.vue";
import Fotter from "./components/Fotter.vue";
</script>
<template>
  <Navbar class="row bg-info-subtle p-0"></Navbar>
  <div class="d-flex">
    <Sidebar></Sidebar>
    <MainContent></MainContent>
  </div>
  <Fotter></Fotter>
</template>
<style></style>
