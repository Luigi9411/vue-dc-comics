<template>
  <div>
    <HeaderPage />

    <MainPage />

    <FooterPage />

    <ArticlePage />
  </div>
</template>

<script>
import HeaderPage from '@/components/HeaderPage.vue';

import MainPage from '@/components/MainPage.vue';

import FooterPage from '@/components/FooterPage.vue';

import ArticlePage from '@/components/ArticlePage.vue';

export default {
  components: {
    HeaderPage,
    MainPage,
    FooterPage,
    ArticlePage,
  },
};
</script>

<style lang="scss">
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
</style>
