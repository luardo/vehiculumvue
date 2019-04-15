<template>
  <div class="section-title">
    <h2 class="section-title__title">{{title}}</h2>
  </div>
</template>

<script>
export default {
  name: "SectionTitle",
  props: {
    title: String
  }
};
</script>
<style lang="scss" scoped>
.section-title {
  display: block;
  padding: 32px 100px;
  &__title {
    text-align: left;
    object-fit: contain;
    font-size: 20px;
    font-weight: 600;
    color: #000000;
  }
}
</style>

