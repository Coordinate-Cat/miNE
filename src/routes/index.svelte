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
  <title>Sapper Blog Template</title>
</svelte:head>

<h1>Oops! You have found this page well. Sorry, This is just a personal page!</h1>
<div class="container">
  <div class="item">
    <img src="apple-1997.jpg" alt="">
    <img src="yahoo.gif" alt="">
    <img src="netscape.gif" alt="">
    <img src="ibm.gif" alt="">
    <img src="internet-ex.gif" alt="">
  </div>
  <div class="item">
    <img src="pentium.gif" alt="">
    <img src="mac-mall.gif" alt="">
    <img src="match-com.gif" alt="">
    <img src="pizza-hut.gif" alt="">
    <img src="postnet.gif" alt="">
  </div>
  <div class="item">
    <img src="mcdonalds.gif" alt="">
    <img src="microsoft.gif" alt="">
    <img src="internet-explorer.gif" alt="">
    <img src="netscape-mini.gif" alt="">
    <img src="quicktime.gif" alt="">
  </div>
</div>
