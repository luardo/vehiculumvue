<template>
  <div class="details-table" :class="modifierClass ? 'details-table--'+modifierClass : ''">
    <div class="details-table__row">
      <div>Avr. cost per month</div>
      <div>€799</div>
    </div>
    <div class="details-table__row">
      <div>Vehiculum price</div>
      <div>€699</div>
    </div>
    <div class="details-table__row details-table__row--featured">
      <div>
        <strong>Saved during deal</strong>
      </div>
      <div>€ 4649</div>
    </div>
  </div>
</template>
<script>
export default {
  name: "DetailsTable",
  props: {
    modifierClass: String
  }
};
</script>

<style lang="scss" scoped>
.details-table {
  &--boxed {
    padding: 28px;
    border-radius: 2px;
    border: solid 1px #e8e8e8;
    background-color: #ffffff;
  }

  &__row {
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: space-between;
    padding: 5px 0;

    &--featured {
      padding-top: 15px;
      font-weight: bold;
    }
  }
}
</style>

