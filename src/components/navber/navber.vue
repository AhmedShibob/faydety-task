<template>
  <div>
    <nav class="navbar" role="navigation" aria-label="main navigation">
      <div class="container">
        <div class="navbar-brand">
          <a class="navbar-item" href="#">
            <img
              src="https://www.faydety.com/assets/images/logos/faydety-colorful.svg"
            />
          </a>

          <a
            role="button"
            class="navbar-burger burger "
            :class="showMobNav ? 'is-active' : ''"
            aria-label="menu"
            aria-expanded="false"
            data-target="navbarBasicExample"
            @click="showMobNav = !showMobNav"
          >
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </a>
        </div>

        <div id="navbarBasicExample" class="navbar-menu">
          <div class="navbar__lists">
            <div class="navber__top-list">
              <ul>
                <li>
                  <a class="navbar-item" href="">
                    How It Works
                  </a>
                </li>
                <li>
                  <a class="navbar-item" href="">
                    Calculators
                  </a>
                </li>
                <li>
                  <a class="navbar-item" href="">
                    Money Blog
                  </a>
                </li>
                <li>
                  <a class="navbar-item" href="">
                    Help Center
                  </a>
                </li>
                <li>
                  <a class="navbar-item" href="">AR</a>
                </li>
                <li class="navber__divider">
                  <div class=""></div>
                </li>
                <li>
                  <a class="navbar-item navber-lang--active" href="">EN</a>
                </li>
              </ul>
            </div>
            <div class="navber__bottom-list">
              <ul>
                <li>
                  <a class="navbar-item" @click="toggleLoans = !toggleLoans">
                    loans
                  </a>
                </li>
                <li>
                  <a class="navbar-item">
                    Credit Cards
                  </a>
                </li>
                <li>
                  <a class="navbar-item">
                    Saving Deposits
                  </a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </nav>
    <div class="header-dropdown" v-if="toggleLoans">
      <div class="container">
        <div class="columns">
          <div class="column is-6 is-offset-2">
            <ul>
              <li>
                <a class="navbar-item">
                  Personal Loans
                </a>
              </li>
              <li class="navber__divider">
                <div class=""></div>
              </li>
              <li>
                <a class="navbar-item">
                  Home Loans
                </a>
              </li>
              <li class="navber__divider">
                <div class=""></div>
              </li>
              <li>
                <a class="navbar-item">
                  Car Loans
                </a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>

    <div :class="showMobNav ? 'navbar-mob--show' : ''" class="navbar-mob ">
      <div class="navbar-mob__content">
        <ul class="navbar-mob__list-top">
          <li>
            <a href="">
              Personal Loans
            </a>
          </li>
          <li>
            <a href="">
              Home Loans
            </a>
          </li>
          <li>
            <a href="">Car Loans</a>
          </li>
          <li>
            <a href="">
              Credit Cards
            </a>
          </li>
          <li>
            <a href="">
              Saving Deposits
            </a>
          </li>
        </ul>

        <ul class="navbar-mob__list-bottom">
          <li>
            <a class="navbar-item" href="">
              How It Works
            </a>
          </li>
          <li>
            <a class="navbar-item" href="">
              Calculators
            </a>
          </li>
          <li>
            <a class="navbar-item" href="">
              Money Blog
            </a>
          </li>
          <li>
            <a class="navbar-item" href="">
              Help Center
            </a>
          </li>
          <li>
            <a class="navbar-item" href="">AR</a>
          </li>
          <li class="navber__divider">
            <div class=""></div>
          </li>
          <li>
            <a class="navbar-item navber-lang--active" href="">EN</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      toggleLoans: false,
      showMobNav: false,
    };
  },
};
</script>
