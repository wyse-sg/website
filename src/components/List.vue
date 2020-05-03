<template>
    <ul class="nav-menu">
        <ListItem
            v-for="nav in navLinks"
            :nav="nav"
            :key="nav.title"
        />
    </ul>
</template>

<script>

import ListItem from '@/components/ListItem.vue';

export default {
  data() {
    return {
      navLinks: [
        { title: 'Home', path: '/' },
        { title: 'About Us', path: '/about' },
        { title: 'Products', path: '/products' },
        // { title: 'Offices', path: '/offices' },
        { title: 'Contact', path: '/contact' },
      ],
    };
  },
  components: {
    ListItem,
  },
};

</script>

<style scoped lang="scss">
  .nav-menu {
    display: flex;
    flex-direction: column;
    justify-content: center;
    // padding: 0 10%;
    padding: 0;
    height: 100%;
    margin: 0;
  }
</style>
