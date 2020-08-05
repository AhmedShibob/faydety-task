<template>
  <div class="loan">
    <article class="media">
      <figure class="media-left loan__avter-big">
        <p class="image is-128x128">
          <img
            src="https://s3.eu-west-1.amazonaws.com/cdn.faydety.com/images/img_1592840843_was4D61rbvkH6yy9qSCkHRotDazBfl.png"
          />
        </p>
      </figure>
      <div class="media-content">
        <div class="content">
          <div class=loan-mob-header> 
            <figure class=" loan__avter-s ">
              <p class="image is-48x48">
                <img
                  src="https://s3.eu-west-1.amazonaws.com/cdn.faydety.com/images/img_1592840843_was4D61rbvkH6yy9qSCkHRotDazBfl.png"
                />
              </p>
            </figure>
            <p class="loan__title">
              <strong>Egyptian Gulf Bank (EG-Bank)</strong>
            </p>
          </div>
          <div class="columns">
            <div class="column is-four-fifths loan__table">
              <table class="table">
                <tbody>
                  <tr>
                    <td class="firt-cell">
                      <h1>Interest Rate <i></i></h1>
                      <p>16.25 % <span>Decreasing</span></p>
                    </td>
                    <td>
                      <h1>Monthly Installment</h1>
                      <p>3,043 <span>LE</span></p>
                    </td>
                    <td>
                      <h1>
                        Admin Fees
                      </h1>
                      <p>2.50 <span>%</span></p>
                    </td>
                  </tr>

                  <transition name="slide-fade">
                    <tr v-if="toggelDetils">
                      <td>
                        <h1 class="loan__title-list">Fees & Costs</h1>

                        <ul>
                          <li>
                            Late Payment Fixed Fees: 0 LE + 4.00% Late Increase
                            Overrate
                          </li>
                          <li>Late Minimum Payment: 50 LE</li>
                          <li>Flat Interest Rate: 10.89 %</li>
                          <li>Early Redemption: 6.00 %</li>
                        </ul>
                      </td>
                      <td>
                        <h1 class="loan__title-list">Requirements</h1>

                        <ul>
                          <li>National ID</li>
                          <li>Utility Bill Issued Within The Last 3 Months</li>
                          <li>
                            HR Letter with hiring date, net salary & current
                            postion
                          </li>
                          <li>
                            Stamped Personal Bank Statement For The Last 6
                            Months
                          </li>
                          <li>
                            Employer Commitment to Transfer Salary to Bank
                          </li>
                          <li>
                            Age Range: 21 - 60 Years
                          </li>
                          <li>
                            Minimum Salary: 1,000 LE
                          </li>
                        </ul>
                      </td>
                      <td>
                        <h1 class="loan__title-list">
                          Third Column if required
                        </h1>
                      </td>
                    </tr>
                  </transition>
                </tbody>
              </table>

              <div class="loan__togge-detils">
                <button @click="toggelDetils = !toggelDetils" class="button">
                  <span v-if="!toggelDetils">More</span> 
                  <span v-if="toggelDetils">less</span> 
                   Details
                  <span>
                    <font-awesome-icon
                      v-if="!toggelDetils"
                      :icon="['fas', 'angle-down']"
                    />
                    <font-awesome-icon
                      v-if="toggelDetils"
                      :icon="['fas', 'angle-up']"
                    />
                  </span>
                </button>
              </div>
            </div>
            <div class="column">
              <div class="loan__action">
                <a href="">Check avilability</a>
                <span>OR</span>
                <button class="button is-rounded">Apply Now</button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </article>
  </div>
</template>

<script>
export default {
  data() {
    return {
      toggelDetils: false,
    };
  },
};
</script>
