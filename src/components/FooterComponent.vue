<template>
  <footer>
    <div id="top_footer">
      <div class="container">
        <div class="row">
          <div class="col-4">
            <div class="comics">
              <h3>DC COMICS</h3>
              <ul>
                <li><a href="">Characters</a></li>
                <li><a href="">Comics</a></li>
                <li><a href="">Movies</a></li>
                <li><a href="">TV</a></li>
                <li><a href="">Games</a></li>
                <li><a href="">Videos</a></li>
                <li><a href="">Shop</a></li>
              </ul>
            </div>
            <div class="comics">
              <h3>SHOP</h3>
              <ul>
                <li><a href="">Shop DC</a></li>
                <li><a href="">Shop DC Collectibles</a></li>
              </ul>
            </div>
          </div>
          <div class="col-4">
            <div class="comics">
              <h3>DC</h3>
              <ul>
                <li><a href="">Terms Of Use</a></li>
                <li><a href="">Privacy policy (New)</a></li>
                <li><a href="">Ad chioces</a></li>
                <li><a href="">Advertising</a></li>
                <li><a href="">Jobs</a></li>
                <li><a href="">Subscription</a></li>
                <li><a href="">Talent Workshops</a></li>
                <li><a href="">CPSC Certificates</a></li>
                <li><a href="">Ratings</a></li>
                <li><a href="">Shop Help</a></li>
                <li><a href="">Contact Us</a></li>
              </ul>
            </div>
          </div>
          <div class="col-4">
            <div class="comics">
              <h3>SITES</h3>
              <ul>
                <li><a href="">DC</a></li>
                <li><a href="">MAD Magazine</a></li>
                <li><a href="">DC Kids</a></li>
                <li><a href="">DC Universe</a></li>
                <li><a href="">DC Power Visa</a></li>
              </ul>
            </div>
          </div>
        </div>
        <!-- row -->
        <div class="image_wrapper"></div>
      </div>
    </div>
    <!-- /#top_footer -->
    <div id="bottom_footer">
      <div class="container">
        <div class="row">
          <div class="signup">
            <button>
              <a href="">SIGN-UP NOW!</a>
            </button>
          </div>
          <div class="social">
            <h3>FOLLOW US</h3>
            <a href="">
              <img src="../assets/footer-facebook.png" alt="" />
            </a>
            <a href="">
              <img src="../assets/footer-twitter.png" alt="" />
            </a>
            <a href="">
              <img src="../assets/footer-youtube.png" alt="" />
            </a>
            <a href="">
              <img src="../assets/footer-pinterest.png" alt="" />
            </a>
            <a href="">
              <img src="../assets/footer-periscope.png" alt="" />
            </a>
          </div>
        </div>
      </div>
    </div>
    <!-- /#bottom_footer -->
  </footer>
  <!-- footer -->
</template>

<script>
</script>

<style lang="scss">
@import "../assets/scss/common.scss";

footer {
  #top_footer {
    background-image: url("../assets/footer-bg.jpg");
    height: 370px;

    .container {
      display: flex;
      justify-content: space-between;
      height: 100%;

      .row {
        width: 40%;
        padding: 3rem 0;

        .comics {
          h3 {
            font-size: 1.3rem;
            color: $color-text-primary;
            margin-bottom: 1rem;
          }
          ul {
            list-style: none;
            margin-bottom: 1rem;

            li {
              a {
                text-decoration: none;
                color: $color-text-secondary;
                font-size: 0.8rem;
                font-weight: bold;
              }
            }
          }
        }
      }
      .image_wrapper {
        width: 50%;
        background-image: url("../assets/dc-logo-bg.png");
        background-position-y: center;
        background-position-x: right;
        background-repeat: no-repeat;
      }
    }
  }
  #bottom_footer {
    background: $color-footer;

    .row {
      justify-content: space-between;
      align-items: center;

      .signup {
        padding: 1.5rem 0;
        button {
          border: 3px solid $color-brand;
          background: $color-footer;
          padding: 0.8rem;

          a {
            color: $color-text-primary;
            text-decoration: none;
            font-size: 1.1rem;
          }
        }
      }
      .social {
        display: flex;
        align-items: center;

        h3 {
          color: $color-brand;
        }

        a {
          margin-left: 1.2rem;
        }
      }
    }
  }
}
</style>