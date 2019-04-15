<template>
  <div class="vehicle-box">
    <div class="vehicle-box__top">
      <div class="vehicle-box__title">
        <h4>Audi Q3</h4>
        <h5>Audi</h5>
      </div>
      <RatingBox title="Attractivnes" :value="5.5"/>
    </div>
    <div class="vehicle-box__image">
      <img :src="carimage">
    </div>
    <div class="vehicle-box__details">
      <DetailsTable/>
    </div>

    <div class="vehicle-box__bottom">This offer is valid only for the next 48 hours. Hurry up!</div>
  </div>
</template>
<script>
import RatingBox from "@/components/atoms/RatingBox.vue";
import carimage from "@/images/bitmap@2x.jpg";
import DetailsTable from "@/components/atoms/DetailsTable.vue";

export default {
  name: "VehicleBox",
  props: {
    brand: String,
    model: String,
    image: String,
    pricePerMonth: Number,
    specialPrice: Number,
    discountAmount: Number,
    disclaimer: String,
    rating: Number
  },
  components: {
    RatingBox,
    DetailsTable
  },
  data() {
    return {
      carimage: carimage
    };
  }
};
</script>
<style lang="scss" scoped>
.vehicle-box {
  width: 295px;
  border-radius: 2px;
  border: solid 1px #efefef;
  background-color: #ffffff;
  padding: 20px;
  text-align: left;
  &__top {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }
  &__title {
    text-align: left;
    h4 {
      font-weight: bold;
      font-size: 18px;
    }
    h5 {
      font-size: 14px;
      font-weight: 300;
      color: #7f7f7f;
    }
  }

  &__image {
    width: 268px;
    height: 179px;
    object-fit: contain;

    img {
      max-width: 100%;
    }
  }

  &__details {
    padding: 5px 0;
  }

  &__bottom {
    padding: 30px 0;
  }
}
</style>
