<template>
  <header class='container'>
    <img src="@/img/dc-logo.png" alt="">
    <nav>
      <ul>
        <li><a href="#!">CHARACTERS</a></li>
        <li><a href="#!">COMICS</a></li>
        <li><a href="#!">MOVIES</a></li>
        <li><a href="#!">TV</a></li>
        <li><a href="#!">GAMES</a></li>
        <li><a href="#!">COLLECTIBLES</a></li>
        <li><a href="#!">VIDEOS</a></li>
        <li><a href="#!">FANS</a></li>
        <li><a href="#!">NEWS</a></li>
        <li><a href="#!">SHOP</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'HeaderPage',
};
</script>

<style lang="scss" scoped>
  header {
    display: flex;
    margin: auto;
    width: 1100PX;
    justify-content: space-between;
    align-items: center;
    text-align: center;

    img{
      margin: 1em 0;
      object-fit: cover;
      width: 5%;
    }
    nav {
      height: 2rem;
      ul {
        display: flex;
        justify-content: center;
        height: 100%;
        list-style: none;
        a {
          display: flex;
          justify-content: center;
          align-items: center;
          padding: 0 .5rem;
          height: 100%;
          color: black;
          text-decoration: none;
          font-size: 0.8em;
          &:hover {
            color: blue;
            border-bottom: 1px solid blue;
          }
        }
      }
    }
  }
</style>
