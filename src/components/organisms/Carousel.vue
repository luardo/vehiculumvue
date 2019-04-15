<template>
  <div class="carousel">
    <div class="carousel__item">
      <VehicleBox/>
    </div>
    <div class="carousel__item">
      <VehicleBox/>
    </div>
    <div class="carousel__item">
      <VehicleBox/>
    </div>
    <div class="carousel__item">
      <VehicleBox/>
    </div>
  </div>
</template>
<script>
import VehicleBox from "@/components/molecules/VehicleBox.vue";
export default {
  name: "VehiclesCarousel",
  props: {
    vehicles: Object
  },
  components: {
    VehicleBox
  }
};
</script>
<style lang="scss" scoped>
.carousel {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  margin-bottom: 30px;
  padding: 0 100px;
}
</style>

