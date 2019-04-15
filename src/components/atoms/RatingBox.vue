<template>
  <div class="rating-box">
    <div class="rating-box__title">{{title}}</div>
    <div class="rating-box__value">{{value}}</div>
  </div>
</template>

<script>
export default {
  name: "RatingBox",
  props: {
    title: String,
    value: Number
  }
};
</script>
<style lang="scss" scoped>
.rating-box {
  display: block;
  width: 77px;
  border-radius: 5px;
  padding: 8px;
  background-color: #f1eade;
  text-align: center;
  color: #000000;

  &__title {
    font-size: 10px;
    text-align: center;
    text-decoration: underline;
  }

  &__value {
    font-size: 16px;
    font-weight: bold;
  }
}
</style>
