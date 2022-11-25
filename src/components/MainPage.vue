<template>
  <main>
    <div>
      <div class="container">
      <h2>Content goes here</h2>
      </div>
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
export default {
  name: 'MainPage',
};
</script>

<style lang="scss" scoped>
  main {
    div{
      background-color:black ;
      .container {
        height: 5em;
        max-width: 1100px;
        display: flex;
        align-items: center;
        color: white;
        margin: 0 auto;
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
