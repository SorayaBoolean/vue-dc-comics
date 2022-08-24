<template>
  <div>
    
    <nav>
        <a href="#">
            <img src="@/assets/img/dc-logo.png" alt="logo">
        </a>

        <ul>
            <li> <a href="#">CHARACTERS</a></li>
            <li> <a href="#">COMICS</a></li>
            <li> <a href="#">MOVIES</a></li>
            <li> <a href="#">TV</a></li>
            <li> <a href="#">GAMES</a></li>
            <li> <a href="#">COLLECTIBLES</a></li>
            <li> <a href="#">VIDEOS</a></li>
            <li> <a href="#">FANS</a></li>
            <li> <a href="#">NEWS</a></li>
            <li> <a href="#">SHOP</a></li>
        </ul>

    </nav>


  </div>
</template>

<script>

    export default {
    name: 'MyHeader'

    }

</script>


<style scoped lang="scss">

  ul {
    display: flex;
    justify-content: space-around;

    li {
      margin: 10px;
      display: flex;
      align-items: center;
      font-size: smaller;
    }
  }
  nav {
    padding: 10px 0px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: auto;
    max-width: 1200px;

    img {
      height: 70px;
      widows: 70px;
    }
  }



</style>
