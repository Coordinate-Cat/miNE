<script>
	export let segment;
</script>

<style>
	nav {
		position: fixed;
    right: 0;
    left: 0;
    z-index: 999;
		margin-bottom: 0;
		background-color: #bbb;
		font-size: 18px;
	}
	ul {
		margin: 0 0 0 20px ;
		padding: 0;
	}
	/* clearfix */
	ul::after {
		content: '';
		display: block;
		clear: both;
	}
	li {
		display: block;
		float: left;
    margin: 0;
	}
	a {
		text-decoration: none;
		padding: 0 10px;
		display: block;
		color: #000;
		background-color: #bbb;
	}
	a:hover {
		color: #bbb;
		background-color: #000;
	}
	a:active {
		color: rgb(255,62,0);
	}
</style>

<nav>
	<ul>
		<li><a class='{segment === undefined ? "selected" : ""}' href='.'>home</a></li>
    <li><a class='{segment === "about" ? "selected" : ""}' href='about'>about</a></li>
    <li><a rel=prefetch class='{segment === "blog" ? "selected" : ""}' href='blog'>blog</a></li>
		<li><a href="https://github.com/Coordinate-Cat" target=”_blank”>Github</a></li>
	</ul>
</nav>