<template>
    <li class="nav-item">
      <router-link class="nav-link" :to="nav.path">{{nav.title}}</router-link>
    </li>
</template>

<script>
export default {
  props: {
    nav: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style lang="scss">
  .nav-item {
    list-style: none;
    margin: 6px;

    .nav-link {
      color: #15330e;
      font-weight: 450;
      font-size: 16px;

      &:hover {
        font-weight: 600;
      }

      &.router-link-active {
        font-weight: 600;
      }
    }
  }
</style>
