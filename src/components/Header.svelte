<script>
  import Nav from './Nav.svelte'

  export let segment
</script>

<style>
  header {
    display: fixed;
  }
</style>

<header>
  <Nav {segment} />
</header>
