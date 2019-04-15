<template>
  <router-link to class="link-item">{{ title }}</router-link>
</template>

<script>
export default {
  name: "LinkItem",
  props: {
    link: Object,
    title: String,
    isActive: Boolean
  }
};
</script>

<style lang="scss" scoped>
.link-item {
  font-family: Montserrat;
  font-size: 18px;
  font-weight: 600;
  text-align: center;
  color: #000000;
  text-decoration: none;
  padding: 0 25px;
}
</style>


