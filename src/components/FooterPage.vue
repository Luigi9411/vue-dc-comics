<template>
  <footer>
    <div>
      <ul>
        <li>
          <h2>DC COMICS</h2>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
          </ul>
          <h2>SHOP</h2>
          <ul>
            <li>Shop DC</li>
            <li>Shop DC Collectibles</li>
          </ul>
        </li>
        <li>
          <h2>DC</h2>
          <ul>
            <li>Terms Of Use</li>
            <li>Privacy policy (New)</li>
            <li>Ad Choices</li>
            <li>Advertising</li>
            <li>Jobs</li>
            <li>Subscriptions</li>
            <li>Talent Workshops</li>
            <li>CPSC Certificates</li>
            <li>Ratings</li>
            <li>Shop Help</li>
            <li>Contact Us</li>
          </ul>
        </li>
        <li>
          <h2>SITES</h2>
          <ul>
            <li>DC</li>
            <li>MAD Magazine</li>
            <li>DC Kids</li>
            <li>DC Universe</li>
            <li>DC Power Visa</li>
          </ul>
        </li>
      </ul>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterPage',
};
</script>

<style lang="scss" scoped>
  footer {
    height: 24em;
    background-image: url('@/img/footer-bg.jpg');
    div{
      width: 1100px;
      margin: 0 auto;
      ul{
        color: white;
        display: flex;
        padding-right: 3em;
        list-style: none;
        li{
          h2{

            padding-top: 1.5em;
            padding-bottom: .5em;
          }
          ul{
            display: flex;
            flex-direction: column;
            li{
              color: #959595;
              list-style: none;
              line-height: 1.3em;
            }

          }
        }
      }
    }
  }
</style>
