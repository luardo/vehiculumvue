<template>
  <div class="title">
    <h1 class="title__main">{{ title }}</h1>
    <h2 v-if="subtitle" class="title__subtitle">{{ subtitle }}</h2>
  </div>
</template>
<script>
export default {
  name: "title",
  props: {
    title: String,
    subtitle: String
  }
};
</script>
<style lang="scss" scoped>
.title {
  text-align: left;
  &__main {
    text-shadow: 1px 1px 1px rgba(214, 214, 214, 0.5);
    font-family: Montserrat;
    font-size: 40px;
    font-weight: 600;
    font-style: normal;
    font-stretch: normal;
    line-height: 1.2;
    letter-spacing: normal;
    color: #ffffff;
    text-transform: uppercase;
  }

  &__subtitle {
    font-family: Montserrat;
    font-size: 20px;
    font-weight: normal;
    font-style: normal;
    font-stretch: normal;
    line-height: 1;
    letter-spacing: normal;
    color: #ffffff;
  }
}
</style>


