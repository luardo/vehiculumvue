<template>
  <header class="header">
    <div class="header__logo">
      <Logo/>
    </div>
    <div class="header__navigation">
      <Navigation/>
    </div>
    <div class="header__column">
      <SecondaryNavigation/>
    </div>
  </header>
</template>

<script>
import Logo from "@/assets/logo.svg?inline";
import CartIcon from "@/assets/cart-icon.svg?inline";

import Navigation from "@/components/molecules/Navigation.vue";
import SecondaryNavigation from "@/components/molecules/SecondaryNavigation.vue";

export default {
  name: "Header",
  components: { Logo, Navigation, CartIcon, SecondaryNavigation }
};
</script>

<style lang="scss" scoped>
.header {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-evenly;
  padding: 0 97px;
  height: 62px;

  &__logo {
    flex-basis: 120px;
  }

  &__navigation {
    flex-grow: 2;
  }
  &__column {
    align-self: center;
  }
}
</style>


