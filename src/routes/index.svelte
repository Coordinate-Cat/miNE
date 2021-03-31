<script>
import Blink from '../components/blink/Blink.svelte';
</script>

<style>
  h2 {
    border: 2px solid #fff;
    width: fit-content;
    margin: 20px 0 0 0;
    line-height: 20px;
    padding: 2px;
    display: flex;
  }
  .container {
    display: flex;
    justify-content: space-between;
    width: 100%;
    height: 100vh;
    margin: 0;
    background-color: #000;
  }
  .web-tree {
    margin: 0 20px;
  }
  /* img {
    max-width: 450px;
    height: auto;
  } */
  @media (max-width:480px) {
  .container {
    flex-wrap: wrap !important;
  }

  .web-tree_item {
      width: auto !important;
  }

}
</style>

<svelte:head>
  <title>miNE</title>
</svelte:head>
<!-- <h1 class="line-1 anim-typewriter">Oops! You have found this page well. Sorry, This is just a personal page!</h1> -->

<div class="container">

  <div class="web-tree">
    <div class="web-tree_item">
      <div class="web-tree_item_profile">
        <h2>miNE<Blink /></h2>
      </div>
    </div>
  </div>

</div>

<!-- <div class="container">
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
</div> -->