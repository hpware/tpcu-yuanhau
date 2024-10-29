<script>
	import { page } from '$app/stores';
</script>
<nav>
	<span>koadasd</span>

	<ul>
<li aria-current={$page.url.pathname === "/" ? "page" : undefined}>
	<a href="/">Home</a>
</li>&nbsp;
<li>
	<a href="/about">About</a>
</li>&nbsp;
<li>
	<a href="/sverdle">Sverdle</a>
</li>
</ul>
</nav>

<style>
	ul {
			text-decoration: none;
			list-style: none;
			display:flex;
			justify-content:center;
			align-items:center;
			padding:0;
			margin:0;
	}
	nav {
			text-align:center;
			display:flex;
			justify-content:center;
			align-items:center;
	}
</style>