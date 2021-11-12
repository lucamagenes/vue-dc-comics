<template>
  <div>
    <div class="card">
      <img :src="image" alt="" />
      <h4>{{ titolo }}</h4>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    image: String,
    titolo: String,
  },
};
</script>

<style lang="scss">
@import "../assets/scss/common.scss";

.card {
  height: 190px;
  margin-bottom: 3rem;
  img {
    max-height: 100%;
    width: 100%;
    object-fit: cover;
    object-position: top;
  }
  h4 {
    color: $color-text-primary;
    padding: 0.5rem 0;
  }
}
</style>