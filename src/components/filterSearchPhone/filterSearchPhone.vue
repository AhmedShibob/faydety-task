<template>
  <section>
    <div class="FilterSearchPhone container">
      <div class="item">
        <p>
          <font-awesome-icon :icon="['fas', 'filter']" />
          <strong>4 Filter</strong>
        </p>
      </div>

      <div class="item">
        <button class="button is-rounded" @click="toggelModel = !toggelModel">
          Change
        </button>
      </div>
    </div>

    <div
      class="modal FilterSearchPhonemodel"
      :class="toggelModel ? 'is-active' : ''"
    >
      <div class="modal-background"></div>
      <div class="modal-content">
        <form action="" class="FilterSearchPhonemodel__form">
          <div class="columns">
            <div class="column ">
              <div class="field">
                <label class="label">Loan Amount</label>
                <div class="control">
                  <input class="input" type="text" placeholder="e.g. 100,000" />
                </div>
              </div>
            </div>
            <div class="column ">
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
            <div class="column ">
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
            <div class="column ">
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

            <div class="column ">
              <button
                class="button is-rounded"
                @click.prevent="toggelModel = !toggelModel"
              >
                Apply Changes
              </button>
            </div>
          </div>
        </form>
      </div>
      <button
        class="modal-close is-large"
        @click="toggelModel = !toggelModel"
        aria-label="close"
      ></button>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      toggelModel: false,
    };
  },
};
</script>
