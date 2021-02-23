<template>
  <div class="dashboard-page-container">
    <b-container class="dashboard-wrapper">
      <b-row>
        <b-container class="top-credit-wrapper mb-3">
          <b-row class="top-credit-wrapper">
            <b-col>
              <b-container class="credit-container">
                <b-row>
                  <b-col>
                    <span class="credit-score align-middle">742</span>
                    <span class="credit-change align-middle">^ 17 points</span>
                    <span class="credit-rating align-middle">Good Credit</span>
                  </b-col>
                  <b-col>
                    Chart
                  </b-col>
                </b-row>
              </b-container>
            </b-col>
          </b-row>
          <b-row>
            <b-col>
              <div class="credit-footer">
                <b-container>
                  <b-row>
                    <b-col class="updated" cols="2">Updated today</b-col>
                    <b-col class="provider" cols="4">
                      VantageScore 3.0 provided by TransUnion
                    </b-col>
                  </b-row>
                </b-container>
              </div>
            </b-col>
          </b-row>
        </b-container>
      </b-row>
      <b-row class="header-wrapper">
        <b-col cols="8">
          <div class="mortgage-standing-wrapper">
            <h4>Tracking your Savings goal</h4>
            <div class="layout-card savings-goal-container mb-4">
              <div class="placeholder"></div>
            </div>

            <h4>Current Mortgage Standing</h4>
            <b-container class="layout-card mortgage-standing-container mb-4">
              <b-row align-v="center">
                <b-col>
                  <div class="mortgage-standing-heading">Current Mortgage Qualification</div>
                </b-col>
                <b-col>
                  <div class="loan-type">Conventional 3% Down</div>
                </b-col>
              </b-row>
              <b-row align-v="center">
                <b-col>
                  <b-container class="mortgage-container">
                    <b-row align-v="center" class="financials-wrapper">
                      <b-col cols="3">
                        <h1>$300k</h1>
                      </b-col>
                      <b-col cols="3">
                        <div class="monthly-payment"><strong>$1260</strong>/mo</div>
                        <div class="interest-rate">2.9% APR</div>
                      </b-col>
                    </b-row>
                  </b-container>
                </b-col>
              </b-row>
              <b-row>
                <b-col>
                  <div class="mortgage-impacts-wrapper">
                    <h5>Negative Impacts</h5>
                    <ul>
                      <li>Credit Score below 740</li>
                      <li>Less than 20% Down Payment</li>
                    </ul>
                  </div>
                </b-col>
              </b-row>
            </b-container>
            <div class="help-with-mortgage-standing mb-4">
              <h4>We can help you get more house by reaching your goals</h4>
            </div>
            <b-container class="layout-card mortgage-standing-container mb-4 positive">
              <b-row>
                <b-col>
                  <div class="mortgage-standing-heading">Potential Mortgage Qualification</div>
                </b-col>
                <b-col>
                  <div class="loan-type">Conventional 10% Down</div>
                </b-col>
              </b-row>
              <b-row align-v="center">
                <b-col>
                  <b-container class="mortgage-container">
                    <b-row align-v="center" class="financials-wrapper">
                      <b-col cols="3">
                        <h1>$315k</h1>
                      </b-col>
                      <b-col cols="3">
                        <div class="monthly-payment"><strong>$1260</strong>/mo</div>
                        <div class="interest-rate">2.5% APR</div>
                      </b-col>
                    </b-row>
                  </b-container>
                </b-col>
              </b-row>
              <b-row>
                <b-col>
                  <div class="mortgage-impacts-wrapper">
                    <h5>Recommended Improvements</h5>
                    <ul>
                      <li>Credit Score at or above 740</li>
                      <li>Pay down Consumer Debts</li>
                    </ul>
                  </div>
                </b-col>
              </b-row>
            </b-container>
            <h4>Renting vs. Buying</h4>
            <b-container class="layout-card mortgage-standing-container mb-4">
              <b-row>
                <b-col>Confused about whether you should continue renting or buying? Here are some Pros and Cons of each. You can also calculate the financial implications using our <a href="#">Rent vs Buy Calculator</a></b-col>
              </b-row>
            </b-container>
          </div>
        </b-col>
        <b-col cols="4">
          <div class="co-buyer-wrapper mb-4">
            <a href="#" class="button">Add Co-Buyer</a>
          </div>
          <h5>How will you use this property?</h5>
          <div class="layout-card questionnaire-wrapper mb-4">
            <div class="option mb-2">Primary Residence</div>
            <div class="option mb-2">Secondary Home</div>
            <div class="option">Rental Property</div>
          </div>
          <h5>Your Current Debts</h5>
          <div class="layout-card current-debts-wrapper mb-4">
            <b-container class="total-debts-container pt-2">
              <b-row align-v="center">
                <b-col>
                  <b-progress :max="100" class="mb-3">
                    <b-progress-bar variant="primary" :value="25" class="credit-card"></b-progress-bar>
                    <b-progress-bar variant="success" :value="30" class="personal-loan"></b-progress-bar>
                    <b-progress-bar variant="info" :value="45" class="auto-loan"></b-progress-bar>
                  </b-progress>
                </b-col>
              </b-row>
              <b-row class="total" align-v="center">
                <b-col cols="1">
                  <div class="dot total-debt"></div>
                </b-col>
                <b-col>Total Debts</b-col>
                <b-col class="value">$17,583</b-col>
              </b-row>
              <b-row align-v="center">
                <b-col cols="1">
                  <div class="dot credit-card"></div>
                </b-col>
                <b-col>Credit Cards</b-col>
                <b-col class="value">$1,583</b-col>
              </b-row>
              <b-row align-v="center">
                <b-col cols="1">
                  <div class="dot personal-loan"></div>
                </b-col>
                <b-col>Personal Loans</b-col>
                <b-col class="value" cols="auto">$4,303</b-col>
              </b-row>
              <b-row align-v="center">
                <b-col cols="1">
                  <div class="dot auto-loan"></div>
                </b-col>
                <b-col>Auto Loans</b-col>
                <b-col class="value">$12,200</b-col>
              </b-row>
              <b-row align-v="center" class="goto-credit-overview-wrapper">
                <b-col>
                  <a href="#">Go to your full Credit Overview</a>
                </b-col>
              </b-row>
            </b-container>
          </div>
          <div class="insight-wrapper">
            <h5>Latest Insights</h5>
            <div class="layout-card">
              <div class="insight-card">
                <div class="title">You are using a high percentage of your available credit</div>
                <div class="body">The less amount of credit you use the more positive impact it will have on your credit score.</div>
              </div>
              <div class="insight-card">
                <div class="title">You are using a high percentage of your available credit</div>
                <div class="body">The less amount of credit you use the more positive impact it will have on your credit score.</div>
              </div>
            </div>
          </div>
        </b-col>
      </b-row>
      <b-row class="mt-4">
        <b-col>
          <h4>Articles</h4>
          <div class="articles-wrapper mb-4">
            <b-card-group columns>
              <b-card
                sub-title="What it’s like to own vs renting and how it can change things"
                img-src="https://picsum.photos/600/300/?image=25"
                img-alt="Image"
                img-top
                tag="article"
                class="mb-2"
              >
                <b-card-text>
                  <small class="text-muted">November 5th, 2020</small>
                </b-card-text>
                <b-button href="#" variant="primary" block>Read Article</b-button>
              </b-card>
              <b-card
                sub-title="What it’s like to own vs renting and how it can change things"
                img-src="https://picsum.photos/600/300/?image=25"
                img-alt="Image"
                img-top
                tag="article"
                class="mb-2"
              >
                <b-card-text>
                  <small class="text-muted">November 5th, 2020</small>
                </b-card-text>
                <b-button href="#" variant="primary" block>Read Article</b-button>
              </b-card>
              <b-card
                sub-title="What it’s like to own vs renting and how it can change things"
                img-src="https://picsum.photos/600/300/?image=25"
                img-alt="Image"
                img-top
                tag="article"
                class="mb-2"
              >
                <b-card-text>
                  <small class="text-muted">November 5th, 2020</small>
                </b-card-text>
                <b-button href="#" variant="primary" block>Read Article</b-button>
              </b-card>
            </b-card-group>
          </div>
        </b-col>
      </b-row>
    </b-container>

  </div>
</template>

<script>

export default {
}
</script>

<style lang="scss" scoped>
.dashboard-page-container {
  background: #eff3f8;
  min-height: 100vh;

  .dashboard-wrapper {
  }

  .layout-card {
    background: #FFF;
    border-radius: 5px;
    box-shadow: 0px 1px 10px rgba(#000, 0.1);
    padding: 15px;
  }

  .top-credit-wrapper {
    .credit-container {
      background: #1761a0;
      padding: 40px 25px;

      .credit-score {
        font-size: 60px;
        font-weight: 200;
        color: #FFF;
      }
      .credit-change {
        font-size: 18px;
        font-weight: 400;
        color: #a5d6a7;
        margin: 0 25px;
      }
      .credit-rating {
        font-size: 16px;
        font-weight: 400;
        background: #4caf50;
        padding: 10px 35px;
        border-radius: 5px;
        color: #FFF;
      }
    }
    .credit-footer {
      padding: 10px 0px;
      background: #4c96d7;
      color: #FFF;

      .updated {
        font-weight: 400;
      }

      .provider {
        font-weight: 400;
        color: #bbdefb;
      }
    }
  }

  .mortgage-standing-wrapper {
    .savings-goal-container {
      background: #192b39;
      .placeholder {
        height: 250px;
      }
    }

    .mortgage-standing-container {
      padding-left: 25px;
      padding-right: 25px;

      .mortgage-standing-heading {
        background: #ededed;
        font-weight: 500;
        padding: 10px;
        text-align: center;
        margin-top: -15px;
        padding-top: 25px;
        font-size: 18px;
        border-bottom-left-radius: 5px;
        border-bottom-right-radius: 5px;
      }

      &.positive {
        background-color: #ecf5f2;
        .mortgage-standing-heading {
          background: #66bb6a;
          color: #FFF;
        }
        h5 {
          color: #66bb6a
        }
      }
    }
    .help-with-mortgage-standing {
      color: #66bb6a;
      font-size: 18px;
      text-align: center;
    }

    .mortgage-container {
      padding: 25px 0;
      h1 {
        font-weight: 300;
      }
    }
    .loan-type {
      text-align: center;
      font-weight: 500;
    }

    .mortgage-impacts-wrapper {
      h5 {
        color: #ff4a4a;
      }
      ul {
        padding-left: 15px;
      }
    }
  }

  .co-buyer-wrapper {
    .button {
      background: #4caf50;
      color: #FFF;
      font-weight: 500;
      font-size: 18px;
      display: block;
      padding: 10px 25px;
      text-align: center;
      border-radius: 5px;
    }
  }

  .current-debts-wrapper {
    .progress {
      border-radius: 25px !important;
      height: 10px;

      .progress-bar {
        &.credit-card {
          background-color: #f39c12 !important;
        }

        &.personal-loan {
          background-color: #4c96d7 !important;
        }

        &.auto-loan {
          background-color: #1abc9c !important;
        }
      }
    }

    .total-debts-container {
      .total {
        border-bottom: solid 1px #eff3f8;
      }
      .value {
        text-align: right;
        font-weight: 500;
      }
      .row {
        padding: 2px 0px;
        .dot {
          height: 14px;
          width: 14px;
          background-color: gray;
          border-radius: 1000px;
        }

        &.goto-credit-overview-wrapper {
          padding: 15px;
          text-align: center;
          border-top: solid 1px #eff3f8;
          margin-top: 10px;
        }
      }
    }
  }

  .questionnaire-wrapper {
    .option {
      font-size: 18px;
      font-weight: 500;
      color: #424242;
      padding: 10px 25px;
      background: #e0e0e0;
      text-align: center;
      border-radius: 5px;
    }
  }

  .insight-wrapper {
    .insight-card {
      border-left: solid 2px #1761a0;
      padding-left: 15px;
      margin-top: 10px;
      margin-bottom: 10px;

      .title {
        font-weight: bold;
        font-size: 16px;
        line-height: 18px;
        margin-bottom: 5px;
      }
      .body {
        font-size: 15px;
        line-height: 18px;
      }
    }
  }
}
</style>
