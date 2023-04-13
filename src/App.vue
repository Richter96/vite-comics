<script>
export default {

}
</script>


<template>
  <header id="app_header">
    <div class="container-md d-flex align-items-center justify-content-between">
      <div class="logo">
        <img src="./assets/img/dc-logo.png" alt="">
      </div>
      <nav class="nav justify-content-center">
        <a class="nav-link active" href="#" aria-current="page">CHARACTERS</a>
        <a class="nav-link " href="#">COMICS</a>
        <a class="nav-link " href="#">MOVIES</a>
        <a class="nav-link " href="#">TV</a>
        <a class="nav-link " href="#">GAMES</a>
        <a class="nav-link " href="#">COLLECTIBLES</a>
        <a class="nav-link " href="#">VIDEOS</a>
        <a class="nav-link " href="#">FANS</a>
        <a class="nav-link " href="#">NEWS</a>
        <a class="nav-link " href="#">SHOP</a>
      </nav>
    </div>
  </header>

  <main id="app_main">
    <div class="container-md align-items-center">
      <p>CONTENT GOES HERE</p>
    </div>
  </main>



  <footer id="app_footer">
    <section class="top_footer">
      <div class=" container-md m-auto row">
        <div class="col">
          <a class=" text-decoration-none" href="">
            <img src="./assets/img/buy-comics-digital-comics.png" alt="">
            <span class="text-white ps-3">DIGITAL COMICS</span>
          </a>
        </div>
        <div class="col">
          <a class=" text-decoration-none" href="">
            <img src="./assets/img/buy-comics-merchandise.png" alt="">
            <span class=" text-white ps-3">DC MERCHANDISE</span>
          </a>
        </div>
        <div class="col">
          <a class=" text-decoration-none" href="">
            <img src="./assets/img/buy-comics-subscriptions.png" alt="">
            <span class=" text-white ps-3">SUBSCRIPTIONS</span>
          </a>
        </div>
        <div class="col">
          <a class=" text-decoration-none" href="">
            <img src="./assets/img/buy-comics-shop-locator.png" alt="">
            <span class=" text-white ps-3">COMIC SHOP LOCATOR</span>
          </a>
        </div>
        <div class="col">
          <a class=" text-decoration-none" href="">
            <img src="./assets/img/buy-dc-power-visa.svg" alt="">
            <span class=" text-white ps-3">DC POWER VISA</span>
          </a>
        </div>

      </div>
    </section>

    <section class="main_footer">
      <div class="row">
        <div class="col">
          <h2>DC </h2>
          <ul>
            li
          </ul>
        </div>
        <div class="col"></div>
        <div class="col"></div>
      </div>
    </section>
    <section class="bottom_footer"></section>


  </footer>
</template>




<style lang="scss" scoped>
// @use './node_modules/bootstrap/scss/bootstrap.scss';

#app_header {
  text-align: center;
  background-color: #ffffff;

  img {
    padding: 1rem;
  }

  a {
    color: black;
    text-decoration: none;
    padding: 0.5rem 1rem;
    border-bottom: 2px solid blue;

    &:not(.active) {
      border-bottom: none;
    }
  }



}


#app_main {
  background-color: #1c1c1c;

  .container-md {
    height: 150px;
    display: flex;
  }


  p {
    color: #ffffff;
  }

}

#app_footer {

  .col {
    margin: 2rem 0;
    font-size: 0.7rem;
    display: flex;
    align-items: center;

    a {
      display: flex;
      align-items: center;
    }
  }

  .top_footer {
    img {
      max-width: 50px;
    }
  }
}
</style>