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
  padding: 20px;
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

a {
  display: block
}
</style>

<svelte:head>
  <title>Blog</title>
</svelte:head>

<div class="container">
  {#each posts as post, index}
    <a rel='prefetch' href='blog/{post.slug}'>
      <div class="post-item">
        <h2>
          {post.title}
        </h2>
        <p>{post.excerpt}</p>
        <div class="post-item-footer">
          <span class="post-item-date">— {post.printDate}</span>
        </div>
      </div>
    </a>
  {/each}
</div>
