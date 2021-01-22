<template>
  <div class="login-page-container">
      <b-container>
        <b-row class="vh-100" align-h="center" align-v="center">
          <b-col cols="6">
            <div class="login-container">
              <h1>Sign In</h1>
              <b-form>
                <b-container>
                  <b-row class="my-3">
                    <b-form-input size="lg" placeholder="Email"></b-form-input>
                  </b-row>
                  <b-row>
                    <b-form-input size="lg" placeholder="Password"></b-form-input>
                  </b-row>
                  <b-row class="mt-3">
                    <b-button type="submit" block size="lg" variant="primary" href="/dashboard">Sign In</b-button>
                  </b-row>
                </b-container>
              </b-form>
            </div>
          </b-col>
        </b-row>
      </b-container>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.login-page-container {
  margin-top: -78px;
  background-image: url("/logo icon.png");
  background-repeat: space;

  .login-container {
    background: #FFF;
    box-shadow: 0px 1px 20px rgba(#000, 0.25);
    padding: 50px;
  }
}
</style>
