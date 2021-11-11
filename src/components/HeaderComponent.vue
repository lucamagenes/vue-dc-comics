<template>
  <header id="site_header">
    <div class="container">
      <div class="logo">
        <img src="../assets/dc-logo.png" alt="" />
      </div>
      <nav>
        <ul>
          <li><a href="">CHARACTERS</a></li>
          <li class="active"><a href="">COMICS</a></li>
          <li><a href="">MOVIES</a></li>
          <li><a href="">TV</a></li>
          <li><a href="">GAMES</a></li>
          <li><a href="">COLLECTIBLES</a></li>
          <li><a href="">VIDEOS</a></li>
          <li><a href="">FANS</a></li>
          <li><a href="">NEWS</a></li>
          <li><a href="">SHOP</a></li>
        </ul>
      </nav>
    </div>
  </header>
  <!-- /#site_header -->
</template>

<script>
</script>

<style lang="scss">
@import "../assets/scss/common.scss";

#site_header {
  width: 100%;
  .container {
    padding: 1.5rem 0;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;

    .logo {
      width: 40%;
    }

    nav {
      width: 60%;
      ul {
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
        list-style: none;

        li {
          padding: 64px 0;

          &.active {
            border-bottom: 4px solid $color-brand;
          }

          &.active a {
            color: $color-brand;
          }

          a {
            text-decoration: none;
            color: black;
            font-size: 0.8rem;
          }
        }
      }
    }
  }
}
</style>