<template>
  <header>
    <b-container>
      <b-row align-v="center">
        <b-col>
          <b-link href="/dev/"><Logo /></b-link>
        </b-col>
        <b-col>
          <b-nav>
            <b-nav-item active>Home</b-nav-item>
            <b-nav-item>Calculators</b-nav-item>
            <b-nav-item>About</b-nav-item>
          </b-nav>
        </b-col>
        <b-col>
          <b-nav pills align="right">
            <b-nav-item href="/dev/login">Login</b-nav-item>
            <b-nav-item active>Sign Up</b-nav-item>
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
