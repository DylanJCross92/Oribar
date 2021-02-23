<template>
  <div class="credit-details-page pt-5">
    <b-container class="tracking-credit-wrapper">
      <b-row>
        <b-col cols="4">
          <div class="layout-card credit-score-wrapper">
            <h5>Tracking your Credit Score</h5>
            <div class="update-in">Updated Today. Next Update in 3 days.</div>
            <img src="credit-score-graph.png" class="graph-example"/>
          </div>
        </b-col>
        <b-col cols="8"><div class="layout-card">Graph</div></b-col>
      </b-row>
    </b-container>
    <b-container class="credit-details-wrapper">
      <b-row>
        <b-col cols="4">
          <div class="layout-card credit-details">
            <div class="eyebrow">Payment History <span class="call-out">Good</span></div>
            <div class="main-text">100%</div>
            <div class="chin">87 payments made on time</div>
            <img class="icon" src="pmt-hist-backdrop.png" />
          </div>
        </b-col>
        <b-col cols="4">
          <div class="layout-card credit-details">
            <div class="eyebrow">Credit Usage <span class="call-out">High</span></div>
            <div class="main-text">25%</div>
            <div class="chin"><strong>$3,459</strong> Credit used of <strong>$13,836</strong> Credit Limit</div>
            <img class="icon" src="credit-usg-backdrop.png" />
          </div>
        </b-col>
        <b-col cols="4">
          <div class="layout-card credit-details">
            <div class="eyebrow">Age of Credit <span class="call-out">Good</span></div>
            <div class="main-text">2 yrs 3 mo</div>
            <div class="chin">3 Accounts More than 5 Years</div>
            <img class="icon" src="age-credit-backdrop.png" />
          </div>
        </b-col>
        <b-col cols="4">
          <div class="layout-card credit-details">
            <div class="eyebrow">Derogatory Marks <span class="call-out">Good</span></div>
            <div class="main-text">0</div>
            <div class="chin">No derogatory marks on your account</div>
            <img class="icon" src="derog-marks-backdrop.png" />
          </div>
        </b-col>
        <b-col cols="4">
          <div class="layout-card credit-details">
            <div class="eyebrow">Total Accounts <span class="call-out">Good</span></div>
            <div class="main-text">14</div>
            <div class="chin">You have a great mix of accounts</div>
            <img class="icon" src="ttl-accnt-backdrop.png" />
          </div>
        </b-col>
        <b-col cols="4">
          <div class="layout-card credit-details">
            <div class="eyebrow">Hard Inquiries <span class="call-out">Medium</span></div>
            <div class="main-text">9</div>
            <div class="chin">Hard inquiries can negatively impact your score </div>
            <img class="icon" src="hard-inqu-backdrop.png" />
          </div>
        </b-col>
      </b-row>
    </b-container>
    <b-container class="debts-wrapper">
      <b-row>
        <b-col cols="8">
          <div class="layout-card">
            <h5>Your Current Debts</h5>
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
                <b-col cols="auto">
                  <div class="dot total-debt"></div>
                </b-col>
                <b-col>Total Debts</b-col>
                <b-col class="value">$17,583</b-col>
              </b-row>
              <b-row align-v="center" class="debt-total">
                <b-col cols="auto">
                  <div class="dot credit-card"></div>
                </b-col>
                <b-col>Credit Cards</b-col>
                <b-col class="value">$1,583</b-col>
              </b-row>
              <b-row align-v="center" class="debt-sub-item">
                <b-col cols="auto">
                  <div class="dot credit-card"></div>
                </b-col>
                <b-col>Chase *7805</b-col>
                <b-col class="value">$1,583</b-col>
              </b-row>
              <b-row align-v="center" class="debt-sub-item">
                <b-col cols="auto">
                  <div class="dot credit-card"></div>
                </b-col>
                <b-col>Bank of America *3925</b-col>
                <b-col class="value">$393</b-col>
              </b-row>
              <b-row align-v="center" class="debt-total">
                <b-col cols="auto">
                  <div class="dot personal-loan"></div>
                </b-col>
                <b-col>Personal Loans</b-col>
                <b-col class="value" cols="auto">$4,303</b-col>
              </b-row>
              <b-row align-v="center" class="debt-sub-item">
                <b-col cols="auto">
                  <div class="dot personal-loan"></div>
                </b-col>
                <b-col>Prosper Financial</b-col>
                <b-col class="value">$16,333</b-col>
              </b-row>
              <b-row align-v="center" class="debt-total">
                <b-col cols="auto">
                  <div class="dot auto-loan"></div>
                </b-col>
                <b-col>Auto Loans</b-col>
                <b-col class="value">$12,200</b-col>
              </b-row>
            </b-container>
          </div>
        </b-col>
        <b-col cols="4">
          <div class="layout-card credit-tips">
            <h5>Credit Tips</h5>
            <div class="body small">
              High credit usage has a negative
              impact on your credit score.
            </div>
            <div class="body mt-2">
              Getting your credit usage down to 5% could have a big impact on your credit score.
            </div>
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
.credit-details-page {
  background: #eff3f8;

  .layout-card {
    background: #FFF;
    border-radius: 5px;
    box-shadow: 0px 1px 10px rgba(#000, 0.1);
    padding: 15px;
    margin-bottom: 25px;

    &.credit-score-wrapper {
      text-align: center;

      .update-in {
        font-size: 14px;
        color: #515b66;
      }

      .graph-example {
        width: 100%;
        margin-top: 25px;
      }
    }

    &.credit-details {
      position: relative;
      z-index: 0;
      .icon {
        content: "";
        position: absolute;
        z-index: -1;
        top: 50%;
        right: 50px;
        height: 80px;
        transform: translateY(-50%);
      }
      .eyebrow {
        font-size: 20px;
        color: #000000;
        .call-out {
          font-size: 15px;
          color: #3edf86;
          margin-left: 10px;
        }
      }
      .main-text {
        font-size: 50px;
        color: #6e71f0;
      }
      .chin {
        font-size: 14px;
        color: #515b66;
      }
    }

    &.credit-tips {
      background: #6e71f0;
      color: #FFF;
    }
  }

  .debts-wrapper {
    .total-debts-container {
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

      .value {
        text-align: right;
        font-weight: 500;
      }

      .row {
        padding: 2px 0px;

        .dot {
          height: 14px;
          width: 14px;
          background: gray;
          border-radius: 1000px;
          margin-right: -20px;

          &.credit-card {
            background: #f39c12;
          }

          &.personal-loan {
            background: #4c96d7;
          }

          &.auto-loan {
            background-color: #1abc9c;
          }
        }
      }

      .debt-total {
        border-top: solid 1px #eff3f8;
        margin-top: 5px;
      }
      .debt-sub-item {
        margin-left: 10px;
      }
    }
  }
}
</style>
