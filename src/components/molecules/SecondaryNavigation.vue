<template>
  <ul class="secondary-navigation">
    <li>
      <CartIcon/>
    </li>
    <li class="secondary-navigation__separator"></li>
    <li>
      <User/>
      <LinkItem title="Your account"/>
    </li>
  </ul>
</template>
<script>
import CartIcon from "@/assets/cart-icon.svg?inline";
import User from "@/assets/user.svg?inline";
import LinkItem from "@/components/atoms/LinkItem.vue";

export default {
  name: "SecondaryNavigation",
  props: {
    navigation: Object
  },
  components: {
    LinkItem,
    CartIcon,
    User
  }
};
</script>

<style lang="scss" scoped>
.secondary-navigation {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  align-items: center;

  li {
    display: flex;
    flex-direction: row;
    align-items: center;
  }

  &__separator {
    height: 36px;
    width: 50px;
    position: relative;

    &::after {
      height: 100%;
      width: 1px;
      content: " ";
      position: absolute;
      right: 50%;
      background-color: #e7e7e7;
    }
  }
}
</style>
