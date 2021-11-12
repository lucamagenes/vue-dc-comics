<template>
  <main id="site_main">
    <div id="main_content">
      <div class="container">
        <div class="row">
          <Thumbnail
            v-for="comic in comics"
            :key="comic.titolo"
            :image="comic.thumb"
            :titolo="comic.series"
            class="col-2"
          />
        </div>
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
import Thumbnail from "./Thumbnail.vue";

export default {
  data() {
    return {
      comics: [
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },
  components: {
    Thumbnail,
  },
};
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