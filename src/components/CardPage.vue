<template>
  <div class="card">
    <img :src="imgUrl" :alt="series">
    <h3>{{title}}</h3>
  </div>
</template>

<script>
export default {
  name: 'CardPage',
  props: {
    imgUrl: {
      type: String,
      required: true,
    },
    title: {
      type: String,
      required: false,
      default: 'Titolo di default',
    },
  },
};

</script>

<style lang="scss" scoped>
   .card {
    padding-top: 3em;
    width: 11em;
    height: 11em;

    img {
      width: 100%;
      height: 100%;
      margin-right: 3em;
      padding-right: 1em;
     }
      h3 {
        font-size: .7rem;
        text-transform: uppercase;
        padding-top: 1em;
      }
}
</style>
