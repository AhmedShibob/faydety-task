<template>
  <section class="filter-search">
    <div class="container">
      <div class="columns is-multiline is-mobile">
        <div class="column is-four-fifths-desktop is-two-thirds-touch">
          <div class="columns is-multiline is-mobile">
            <div class="column is-one-quarter-widescreen is-half-desktop is-half-touch">
              <div class="field">
                <label class="label">Loan Amount</label>
                <div class="control">
                  <input class="input" type="text" placeholder="e.g. 100,000" />
                </div>
              </div>
            </div>
            <div class="column is-one-quarter-widescreen is-half-desktop is-half-touch">
              <div class="field">
                <label class="label">Loan Duration</label>
                <div class="columns is-mobile filter-search__duration">
                  <div class="column column-1">
                    <div class="control">
                      <div class="select">
                        <select>
                          <option v-for="n in 10" :key="n + 'year'">
                            {{ n }} Yrs</option
                          >
                        </select>
                      </div>
                    </div>
                  </div>
                  <div class="column column-2">
                    <div class="control">
                      <div class="select">
                        <select>
                          <option v-for="n in 12" :key="n + 'month'">
                            {{ n }} Mts</option
                          >
                        </select>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="column is-one-quarter-widescreen is-half-desktop is-half-touch">
              <div class="field">
                <label class="label">Employment Type</label>
                <div class="control">
                  <div class="select">
                    <select>
                      <option disabled>
                        Select Employment Type
                      </option>
                      <option>
                        Professional
                      </option>
                      <option>
                        Self Employed
                      </option>
                      <option>
                        Employee
                      </option>
                    </select>
                  </div>
                </div>
              </div>
            </div>
            <div class="column is-one-quarter-widescreen is-half-desktop is-half-touch">
              <div class="field">
                <label class="label">Salary Transfer Status</label>
                <div class="control">
                  <div class="select">
                    <select>
                      <option disabled>
                        Select Salary Transfer Status
                      </option>
                      <option>
                        Full Salary Transfer
                      </option>
                      <option>
                        Installment Transfer Only
                      </option>
                      <option>
                        No Salary Transfer
                      </option>
                    </select>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="column is-one-fifth-desktop is-one-thirds-touch">
          <button class="button is-rounded">change</button>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>
