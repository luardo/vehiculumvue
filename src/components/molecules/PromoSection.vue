<template>
  <div class="promo-section">
    <div class="promo-section__column">
      <div class="promo-section__title">OFFER OF THE MONTH</div>
      <div class="promo-section__subtitle">Ford Mondero 1.5 Eco Boost</div>
    </div>
    <div class="promo-section__column">
      <RatingBox title="Attractivnes" :value="5.5"/>
    </div>
  </div>
</template>
<script>
import RatingBox from "@/components/atoms/RatingBox.vue";

export default {
  name: "PromoSection",
  components: {
    RatingBox
  }
};
</script>
<style lang="scss" scoped>
.promo-section {
  background-color: #000000;
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  padding: 20px 100px;
  align-content: center;
  color: #ffffff;
  &__column {
    padding-right: 38px;
  }

  &__title {
    font-size: 24px;
    font-weight: 600;
    text-transform: uppercase;
  }
  &__subtitle {
    font-size: 20px;
    font-weight: 600;
  }
}
</style>

