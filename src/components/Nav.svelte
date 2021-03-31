<script>
export let segment;

onMount(() => {
  var myVar = setInterval(function() {
    getFormattedTime();
  }, 1);
  function getFormattedTime(date) {
    var d = date || new Date();
    var z = n => ('0'+n).slice(-2);
    var zz = n => ('00'+n).slice(-3);
    document.getElementById("clock").innerHTML =
    `${z(d.getHours())}:${z(d.getMinutes())}:${z(d.getSeconds())}:${zz(d.getMilliseconds())}`;
  }
});

import { onMount } from "svelte";
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
	margin: 0 0 0 10px ;
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
	color: #000;
}
a {
	text-decoration: none;
	padding: 0 10px;
	display: block;
	color: #000;
	background-color: #bbb;
}
a:hover {
	color: rgb(255,62,0);
	background-color: #000;
}
a:active {
	color: rgb(255,62,0);
}
i {
	margin-left: 3px;
	font-size: 12px;
}
#clock {
	padding: 0 5px;
	color: #bbb;
	background-color: #000;
}
#clock::before {
	content: 'JST:'
}
#clock:hover {
	color: rgb(255,62,0);
	cursor: pointer;
}
@media (max-width:480px) {
  #clock {
		display: none;
	}
}
</style>

<nav>
	<ul>
		<li><a class='{segment === undefined ? "selected" : ""}' href='.'>home</a></li>
    <li><a class='{segment === "about" ? "selected" : ""}' href='about'>about</a></li>
    <li><a rel=prefetch class='{segment === "blog" ? "selected" : ""}' href='blog'>blog</a></li>
		<li><a href="https://github.com/Coordinate-Cat" target=”_blank”>Github<i class="fas fa-external-link-alt"></i></a></li>
		<li><p id="clock"></p></li>
	</ul>
</nav>