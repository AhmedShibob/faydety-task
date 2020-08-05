<template>
  <footer class="footer">
    <div class="container">
      <nav class="level">
        <div class="level-left">
          <div class="level-item">
            <img
              src="https://www.faydety.com/assets/images/logos/faydety-colorful.svg"
            />
          </div>
        </div>

        <div class="level-right">
          <ul>
            <li>
              <a class="level-item" href="">
                How It Works
              </a>
            </li>
            <li>
              <a class="level-item" href="">
                Calculators
              </a>
            </li>
            <li>
              <a class="level-item" href="">
                Money Blog
              </a>
            </li>
            <li>
              <a class="level-item" href="">
                Help Center
              </a>
            </li>
          </ul>
        </div>
      </nav>

      <div class="columns">
        <div class="column">
          <div class="columns footer__list">
            <div class="column">
              <h1>Loans</h1>
              <ul>
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
                  <a href="">
                    Car Loans
                  </a>
                </li>
              </ul>
            </div>
            <div class="column">
              <h1>Credit Cards</h1>
              <ul>
                <li>
                  <a href="">
                    Credit Cards
                  </a>
                </li>
              </ul>
            </div>
            <div class="column">
              <h1>Saving Deposits</h1>
              <ul>
                <li>
                  <a href="">
                    Saving Deposits
                  </a>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="column">
          <div class="footer__social-media">
            <ul>
              <li>
                <a href="">
                  <font-awesome-icon :icon="['fab', 'linkedin-in']" />
                </a>
              </li>
              <li>
                <a href="">
                  <font-awesome-icon :icon="['fab', 'instagram']" />
                </a>
              </li>
              <li>
                <a href="">
                  <font-awesome-icon :icon="['fab', 'youtube']" />
                </a>
              </li>
              <li>
                <a href="">
                  <font-awesome-icon :icon="['fab', 'twitter']" />
                </a>
              </li>
              <li>
                <a href="">
                  <font-awesome-icon :icon="['fab', 'facebook']" />
                </a>
              </li>
            </ul>
          </div>
        </div>
      </div>

      <div class="columns footer__bottom-list">
        <div class="column">
          <ul>
            <li>
              <a href="">
                Legal Disclaimer
              </a>
            </li>
            <li>
              <a href="">
                Privacy Policy
              </a>
            </li>
          </ul>
        </div>

        <div class="column">
          <button class="button footer__help-btn">
            <span>
              <font-awesome-icon :icon="['far', 'comment']" />
            </span>
            Help?
          </button>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {};
</script>
