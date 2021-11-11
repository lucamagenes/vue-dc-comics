<template>
  <main id="site_main">
    <div id="main_content">
      <div class="container">
        <h1>Content goes here</h1>
      </div>
    </div>
    <!-- main content -->
    <div id="digital_comics">
      <div class="container">
        <ul>
          <li>
            <a href="">
              <img src="../assets/buy-comics-digital-comics.png" alt="" />
              DIGITAL COMICS
            </a>
          </li>
          <li>
            <a href="">
              <img src="../assets/buy-comics-merchandise.png" alt="" />
              DC MERCHANDISE
            </a>
          </li>
          <li>
            <a href="">
              <img src="../assets/buy-comics-subscriptions.png" alt="" />
              SUBSCRIPTION
            </a>
          </li>
          <li>
            <a href="">
              <img src="../assets/buy-comics-shop-locator.png" alt="" />
              COMIC SHOP LOCATOR
            </a>
          </li>
          <li>
            <a href="">
              <img
                src="../assets/buy-dc-power-visa.svg"
                alt=""
                style="height: 40px"
              />
              DC POWER VISA
            </a>
          </li>
        </ul>
        <!-- lista digital -->
      </div>
    </div>
    <!-- digital comics -->
  </main>
</template>

<script>
</script>

<style lang="scss">
@import "../assets/scss/common.scss";

#site_main {
  #main_content {
    background: $color-main;

    .container {
      padding: 3rem 0;

      h1 {
        color: $color-text-primary;
      }
    }
  }

  #digital_comics {
    background: $color-brand;

    .container {
      padding: 3rem 0;

      ul {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        align-items: center;
        list-style: none;

        li {
          a {
            display: flex;
            align-items: center;
            color: $color-text-primary;
            text-decoration: none;

            img {
              height: 50px;
              margin-right: 1rem;
            }
          }
        }
      }
    }
  }
}
</style>