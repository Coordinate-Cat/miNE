<style>
  .container {
    display: flex;
    margin-top: 20px;
    width: 100%;
  }
  .item2 {
    margin: 0 20px;
  }
  .item3 {
    width: 100%;
  }
  img {
    max-width: 450px;
    height: auto;
  }
  @media (max-width: 1020px) {
    /* p {
      font-size: 1.2em;
    } */
  }

  @media (max-width: 800px) {
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
  <div class="item2">
    <img src="pentium.gif" alt="">
    <img src="mac-mall.gif" alt="">
    <img src="match-com.gif" alt="">
    <img src="pizza-hut.gif" alt="">
    <img src="postnet.gif" alt="">
  </div>
  <div class="item3">
    <img src="mcdonalds.gif" alt="">
    <img src="internet-explorer.gif" alt="">
    <img src="netscape-mini.gif" alt="">
    <img src="quicktime.gif" alt="">
    <img src="microsoft.gif" alt="">
  </div>
</div>
