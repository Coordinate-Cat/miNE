<script context="module">
  export function preload({ params, query }) {
    return this.fetch(`blog.json`).then(r => r.json()).then(posts => {
      return { posts };
    });
  }
</script>

<script>
  export let posts;
</script>

<style>
.post-item {
  border: solid 8px #000;
  padding: 10px;
  margin: 8px 0;
}

.post-item-date {
  color: #AAA;
  text-align: left;
  text-transform: uppercase;
  margin-right: 16px;
}

p {
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}
</style>

<svelte:head>
  <title>Blog</title>
</svelte:head>

<div class="container">
  <h1>Blog</h1>
  {#each posts as post, index}
    <div class="post-item">
      <h2>
        <a rel='prefetch' href='blog/{post.slug}'>{post.title}</a>
      </h2>
      <p>{post.excerpt}</p>
      <div class="post-item-footer">
        <span class="post-item-date">— {post.printDate}</span>
      </div>
    </div>
  {/each}
</div>
