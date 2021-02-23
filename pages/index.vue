<template>
  <div class="home-container">
    <div class="bg-header-wrapper">
      <b-container class="header-content">
        <b-row align-v="center" class="header-wrapper">
          <b-col>
            <h1>Let us help <strong>you own your</strong> future</h1>
            <div class="sub-title">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Quis ipsum suspendisse ultrices gravida accumsan lacus facilisis. </div>
            <b-button variant="success">See how we can help</b-button>
          </b-col>
          <b-col>
            <img class="header-app-photo" src="home/header-app-photo.png"/>
          </b-col>
        </b-row>
      </b-container>
    </div>
    <b-container class="how-we-help">
      <h2>How we can help</h2>
      <div class="sub-title">At Oribar we believe in Lorem ipsum dolor sit amet, </br>consectetur adipiscing elit, sed do eiusmod tempor incididunt.</div>

      <b-row align-v="start" class="help-cols">
        <b-col>
          <img src="home/target.svg" class="icon"/>
          <h3>Set a goal</h3>
          <div class="sub-title">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.
          </div>
          <b-button variant="outline-primary">Set a goal now</b-button>
        </b-col>
        <b-col>
          <img src="home/strategy.svg" class="icon"/>
          <h3>Create a plan</h3>
          <div class="sub-title">
            Ipsum dolor sit amet, consectetur  sed do eiusmod elit. sed do eiusmod el.
          </div>
          <b-button variant="outline-primary">Create a plan now</b-button>
        </b-col>
        <b-col>
          <img src="home/route.svg" class="icon"/>
          <h3>Track your progress</h3>
          <div class="sub-title">
            Ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod adipiscing elit.
          </div>
          <b-button variant="outline-primary">Track your goal</b-button>
        </b-col>
        <b-col>
          <img src="home/celebrate.svg" class="icon"/>
          <h3>Celebrate</h3>
          <div class="sub-title">
            Ipsum dolor sit amet, adipiscing elit, sed do eiusmod el.  sed do eiusmod el.
          </div>
          <b-button variant="outline-primary">Celebrate</b-button>
        </b-col>
      </b-row>
    </b-container>
    <div class="steps-to-buy">
      <b-container>
        <h2>Steps to buy a house</h2>
        <div class="sub-title">There are several steps to buy a house as listed below. </br> See the options available to you.</div>
        <b-row align-v="center" class="steps-container mt-5">
          <b-col>
            <ul class="list">
              <li><b-badge pill variant="primary">1</b-badge> Find the right mortgage program.</li>
              <li><b-badge pill variant="primary">2</b-badge> Determine how much house you can afford.</li>
              <li><b-badge pill variant="primary">3</b-badge> Calculate your down payment.</li>
            </ul>
          </b-col>
          <b-col>
            <img src="home/JumbledWords.png" class="jumbled-words"/>
          </b-col>
        </b-row>
        <b-row class="mt-5">
          <b-col>
            <b-button variant="primary" size="lg">Go to our calculators</b-button>
          </b-col>
        </b-row>
      </b-container>
    </div>
    <b-container class="alternating-info">
      <b-row class="mt-5" align-v="center">
        <b-col cols="3">
          <img src="home/placeholder-app.png" class="app-image"/>
        </b-col>
        <b-col>
          <h3>Setting a goal</h3>
          <div class="body">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan lacus vel facilisis. </div>
          <ol class="mt-3">
            <li>We’ll help you <a href="#">determine how much house you can afford</a>.</li>
            <li>Then determine what steps you need to take.</li>
            <li>Move on to <a href="#">creating a plan</a> to execute.</li>
          </ol>
        </b-col>
      </b-row>
      <b-row class="mt-5" align-v="center">
        <b-col>
          <h3>Creating a plan</h3>
          <div class="body">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan lacus vel facilisis. </div>
          <ol class="mt-3">
            <li>We’ll help you <a href="#">determine how much house you can afford</a>.</li>
            <li>Then determine what steps you need to take.</li>
            <li>Move on to <a href="#">tracking your steps</a> to execute.</li>
          </ol>
        </b-col>
        <b-col cols="3">
          <img src="home/placeholder-app.png" class="app-image"/>
        </b-col>
      </b-row>
      <b-row class="mt-5" align-v="center">
        <b-col cols="3">
          <img src="home/placeholder-app.png" class="app-image"/>
        </b-col>
        <b-col>
          <h3>Tracking your progress</h3>
          <div class="body">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas accumsan lacus vel facilisis. </div>
          <ol class="mt-3">
            <li>We’ll help you <a href="#">keep track of your progress</a>.</li>
            <li>Then determine what changes you may need to make.</li>
            <li>Lorem ipsum maecenas accumsan lacus vel.</li>
          </ol>
        </b-col>
      </b-row>
    </b-container>
    <b-container style="height: 100px"></b-container>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.home-container {
  .bg-header-wrapper {
    background-size: cover;
    background: url("/home/home-bg-img.jpg");
    background-position: center;
    position: relative;

    &:after {
      content: "";
      position: absolute;
      display: block;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: rgba(#1761a0, 0.95);
      z-index: 1;
    }

    .header-content {
      position: relative;
      z-index: 2;
      .header-wrapper {
        min-height: 60vh;
        padding: 50px 0;

        h1 {
          color: #FFF;
          font-size: 44px;
          font-weight: 200;
        }

        .sub-title {
          color: #FFF;
          font-size: 20px;
          line-height: 24px;
          margin: 15px 0;
        }

        .header-app-photo {
          width: 500px;
          float: right;
        }
      }
    }
  }

  .how-we-help {
    padding: 50px 0;

    .help-cols {
      margin-top: 50px;
      .col {
        .icon {
          height: 50px;
          margin-bottom: 10px;
        }
        .sub-title {
          margin-bottom: 10px;
        }
      }
    }
  }

  .steps-to-buy {
    padding: 50px 0;
    background: #eff3f8;

    .steps-container {
      .jumbled-words {
        max-width: 350px;
      }

      .list {
        font-size: 22px;
        line-height: 28px;
        color: #2c3238;
        margin: 0px;
        padding: 0px;

        li {
          list-style: none;
          margin-bottom: 10px;
          margin-top: 10px;
        }
      }
    }
  }

  .alternating-info {
    .app-image {
      width: 220px;
    }
  }
}
</style>
