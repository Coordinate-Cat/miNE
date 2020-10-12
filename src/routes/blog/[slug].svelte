<script context="module">
  export async function preload({ params, query }) {
    // the `slug` parameter is available because
    // this file is called [slug].html
    const res = await this.fetch(`blog/${params.slug}.json`);
    const data = await res.json();

    if (res.status === 200) {
      return { post: data };
    } else {
      this.error(res.status, data.message);
    }
  }
</script>

<script>
  import Bio from '../../components/Bio.svelte'
  export let post
</script>

<style>
  header {
    text-align: center;
  }

  header h1 {
    margin-bottom: 0.7em;
  }

  header p {
    color: #AAA;
    text-transform: uppercase;
    font-weight: 600;
  }
</style>

<svelte:head>
  <title>{post.title}</title>
</svelte:head>

<div class="container">
  <header>
    <p>{post.printDate} - {post.printReadingTime}</p>
    <h1>{post.title}</h1>
  </header>
  <article class="content">
    {@html post.html}
  </article>
  <hr />
  <Bio />
</div>
