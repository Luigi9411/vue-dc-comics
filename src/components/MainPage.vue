<template>
  <main>
    <div class="back-img"></div>
    <div class="container">
       <div class="title-img">CURRENT SERIES</div>
       <CardPage
        v-for="objCard in arrDc"
        :key="objCard.price"
        :img-url="objCard.thumb"
        :title="objCard.series"
        />
      </div>
      <div class="container-button">
        <button>LOAD MORE</button>
      </div>
    <div class="list">
      <ul>
        <li>
          <img class="shop" src="@/img/buy-comics-digital-comics.png" alt="error">
          <h3>DIGITAL COMICS</h3>
        </li>
        <li>
          <img class="shop" src="@/img/buy-comics-merchandise.png" alt="error">
          <h3>DC MERCHANDISE</h3>
        </li>
        <li>
          <img class="shop" src="@/img/buy-comics-subscriptions.png" alt="error">
          <h3>SUBSCRIPTION</h3>
        </li>
        <li>
          <img class="shop" src="@/img/buy-comics-shop-locator.png" alt="error">
          <h3>COMIC SHOP LOCATOR</h3>
        </li>
        <li>
          <img class="visa" src="@/img/buy-dc-power-visa.svg" alt="error">
          <h3>DC POWER VISA</h3>
        </li>
      </ul>
    </div>
  </main>
</template>

<script>
import CardPage from '@/components/CardPage.vue';

export default {
  name: 'MainPage',
  components: {
    CardPage,
  },
  data() {
    return {
      arrDc: [
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX',
          price: '$19.99',
          series: 'Action Comics',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01',
          price: '$3.99',
          series: 'American Vampire 1976',
          type: 'cmic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb',
          price: '$16.9',
          series: 'Aquaman',
          type: 'grapic novel',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76',
          price: '$2.99',
          series: 'Batgirl',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
          price: '$399',
          series: 'Baman',
          type: 'comc book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
          price: '$2.99',
          series: 'Batman Beyond',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8',
          price: '$3.99',
          series: 'Batman/Superman',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk',
          price: '$4.99',
          series: 'Batman/Superman Annual',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8',
          price: '$5.99',
          series: 'Batman: The Joker War Zone',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY',
          price: '$6.99',
          series: 'Batman: Three Jokers',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX',
          price: '$4.99',
          series: 'Batman: White Knight Presents: Harley Quinn',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq',
          price: '$16.99',
          series: 'Catwoman',
          type: 'graphic novel',
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
  main {
      .back-img{
        height: 14em;
        background-position: top;
        background-repeat: no-repeat;
        background-size: 100% 270%;
        background-image: url('@/img/jumbotron.jpg');
      }
      background-color: black;
      .container {
        height: 30em;
        max-width: 1100px;
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        color: white;
        margin: 0 auto;
        padding: 1em 0;
        position: relative;
        .title-img{
          position: absolute;
          top: -1em;
          width: 160px;
          background-color: #0282F9;
          color: white;
          white-space: nowrap;
          padding: .5em 1em;
          text-align: center;
        }
      }
      .container-button{
        display: flex;
        justify-content: center;
        margin-top: 2em;
        margin-bottom: 1em;
        button{
        width: 200px;
        background-color: #0282F9;
        color: white;
        white-space: nowrap;
        padding: .5em .5em;
        cursor: pointer;
       }
      }
    .list {
      height: 6em;
      background-color: #0282F9;
      display: flex;
      align-items: center;
      ul{
        width: 1050px;
        margin: 0 auto;
        display: flex;
        gap: 2em;
        li{
          display: flex;
          align-items: center;
          font-size: .6em;
          white-space: nowrap;
          .shop{
            width: 24%;
            padding-right: .5em;
          }
          .visa{
            width: 14%;
            padding-right: .5em;
            margin-left: 3em;
          }
          h3{
            color: white;
          }
        }
      }
    }
  }
</style>
