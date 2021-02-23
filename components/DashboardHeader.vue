<template>
  <header>
    <b-container>
      <b-row align-v="center">
        <b-col>
          <b-link href="/dev/"><Logo /></b-link>
        </b-col>
        <b-col>
          <b-nav>
            <b-nav-item href="/dev/dashboard"active>Dashboard</b-nav-item>
            <b-nav-item href="/dev/dashboard/credit-score">Credit Score</b-nav-item>
            <b-nav-item href="/dev/dashboard/savings">Savings</b-nav-item>
          </b-nav>
        </b-col>
        <b-col>
          <b-nav pills align="right">
            Logged In
          </b-nav>
        </b-col>
      </b-row>
    </b-container>
  </header>
</template>

<style lang="scss" scoped="scoped">
header {
  background: #FFF;
  padding: 10px 0;
  box-shadow: 0px 1px 10px rgba(#000, 0.25);
  position: sticky;
}
</style>
