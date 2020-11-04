<script>
  import Header from '../components/Header.svelte';

  export let segment;
</script>

<style>
  .layout {
    display: flex;
    flex-direction: column;
    min-height: 100%;
    min-height: 100vh;
  }

  main {
    flex: 1;
    position: relative;
    margin: 0 auto;
    margin-top: 20px;
    box-sizing: border-box;
    width: 100%;
    display: flex;
    flex-direction: column;
  }
</style>

<div class="layout">
  <Header {segment}/>

  <main>
    <slot></slot>
  </main>
</div>
