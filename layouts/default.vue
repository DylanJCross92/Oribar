<template>
<div class="page-container">
    <Header v-if="!checkIfDashboard"/>
    <DashboardHeader v-if="checkIfDashboard"></DashboardHeader>
    <Nuxt />
  </div>
</template>

<script>
export default {
  computed: {
    checkIfDashboard() {
      return this.$route.path === "/dashboard" || this.$route.path === "/dashboard/credit-score" || this.$route.path === "/dashboard/savings"
    }
  }
}
</script>

<style>
html {
  font-family:
    'Open Sans',
    'Helvetica Neue',
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}
</style>
