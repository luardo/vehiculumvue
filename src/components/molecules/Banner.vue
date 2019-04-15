<template>
  <div class="banner">
    <div class="banner__image">
      <div
        style="background-image: url(https://images.unsplash.com/photo-1503376780353-7e6692767b70?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2100&q=80)"
      ></div>
    </div>
    <div class="banner__content">
      <slot></slot>
    </div>
  </div>
</template>

<script>
import Title from "@/components/atoms/Title.vue";
import Button from "@/components/atoms/Button.vue";
export default {
  name: "Banner",
  components: {
    Title,
    Button
  }
};
</script>
<style lang="scss" scoped>
.banner {
  width: 100%;
  background: #000000;
  height: 460px;
  object-fit: contain;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  position: relative;
  margin-bottom: 17px;

  &__image {
    position: absolute;
    top: 0;
    left: 0;
    z-index: 0;
    height: 100%;
    width: 100%;
    display: block;

    div {
      width: 100%;
      height: 100%;
      display: block;
      -o-object-fit: cover;
      object-fit: cover;
      background-position: 50% 50%;
      background-repeat: no-repeat;
      background-size: cover;
      font-family: "object-fit: cover;";
    }
  }

  &__content {
    width: 800px;
    padding: 0 97px;
    z-index: 1;

    &::after {
      content: "";
      background: rgba(27, 27, 27, 0.6);
      position: absolute;
      left: 0;
      right: 0;
      top: 0;
      bottom: 0;
      z-index: -1;
    }
  }

  &__buttons-container {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    margin-top: 32px;
  }
}
</style>


