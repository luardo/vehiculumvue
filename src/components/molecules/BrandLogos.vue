<template>
  <div class="brand-logos">
    <div class="brand-logos__item">
      <bmw/>
    </div>
    <div class="brand-logos__item">
      <ford/>
    </div>
    <div class="brand-logos__item">
      <toyota/>
    </div>
    <div class="brand-logos__item">
      <renault/>
    </div>
  </div>
</template>
<script>
import bmw from "@/assets/bmw.svg?inline";
import ford from "@/assets/ford.svg?inline";
import renault from "@/assets/renault.svg?inline";
import toyota from "@/assets/toyota.svg?inline";

export default {
  name: "BrandLogos",
  components: {
    bmw,
    toyota,
    renault,
    ford
  }
};
</script>
<style lang="scss" scoped>
.brand-logos {
  display: flex;
  padding: 25px 100px 55px;
  flex-direction: row;
  flex-wrap: wrap;
  align-items: center;
  justify-content: flex-start;
  text-align: left;

  &__item {
    min-width: 300px;
  }
}
</style>
