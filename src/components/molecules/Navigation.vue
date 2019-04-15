<template>
  <ul class="navigation">
    <li>
      <LinkItem title="Special offers"/>
    </li>
    <li>
      <LinkItem title="Browse vehicles"/>
    </li>
    <li>
      <LinkItem title="About us"/>
    </li>
  </ul>
</template>

<script>
import LinkItem from "@/components/atoms/LinkItem.vue";
export default {
  name: "Navigation",
  props: {
    navigationTree: Object
  },
  components: {
    LinkItem
  }
};
</script>

<style lang="scss" scoped>
.navigation {
  display: flex;
  flex-direction: row;
  justify-content: center;
  padding: 22px;
  list-style: none;
}
</style>


