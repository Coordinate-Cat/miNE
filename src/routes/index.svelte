<style>
  .container {
    display: flex;
    justify-content: space-between;
    margin-top: 20px;
    width: 100%;
  }
  img {
    max-width: 450px;
    height: auto;
  }
  @media (max-width:480px) {
  .container {
    flex-wrap: wrap !important;
  }

  .item {
      width: auto !important;
  }

  img {
    max-width: 100%;
    height: auto;
  }
}
</style>

<svelte:head>
  <title>miNE</title>
</svelte:head>

<h1>Oops! You have found this page well. Sorry, This is just a personal page!</h1>
<div class="container">
  <div class="item">
    <img src="./gif/apple-1997.jpg" alt="">
    <img src="./gif/yahoo.gif" alt="">
    <img src="./gif/netscape.gif" alt="">
    <img src="./gif/ibm.gif" alt="">
    <img src="./gif/internet-ex.gif" alt="">
  </div>
  <div class="item">
    <img src="./gif/pentium.gif" alt="">
    <img src="./gif/mac-mall.gif" alt="">
    <img src="./gif/match-com.gif" alt="">
    <img src="./gif/pizza-hut.gif" alt="">
    <img src="./gif/postnet.gif" alt="">
  </div>
  <div class="item">
    <img src="./gif/mcdonalds.gif" alt="">
    <img src="./gif/microsoft.gif" alt="">
    <img src="./gif/internet-explorer.gif" alt="">
    <img src="./gif/netscape-mini.gif" alt="">
    <img src="./gif/quicktime.gif" alt="">
  </div>
</div>
