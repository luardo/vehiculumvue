<template>
  <a class="button" :class="classNames">{{title}}</a>
</template>
<script>
export default {
  name: "Button",
  props: {
    title: String,
    modifierClass: String,
    modifierClasses: Array
  },
  computed: {
    classNames: function() {
      if (this.modifierClasses) {
        return this.modifierClasses.map(name => "button--" + name);
      }

      return "";
    }
  }
};
</script>

<style lang="scss" scoped>
.button {
  background: #cfb995;
  width: 100%;
  max-width: 295px;
  font-family: Montserrat;
  font-size: 14px;
  font-weight: bold;
  text-align: center;
  color: #ffffff;
  text-transform: uppercase;
  text-align: center;
  padding: 17px 20px;
  display: block;
  &--fullwidth {
    max-width: 100%;
  }

  &--ghost {
    background: none;
    border: solid 1px #ffffff;
  }

  &--red {
    background-color: #fa454b;
  }
}
</style>

