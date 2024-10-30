<script>
	import { page } from '$app/stores';
</script>
<nav>
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
  ul {
      position: relative;
      padding: 0;
      margin: 0;
			height:30px;
      display: flex;
      justify-content: center;
      align-items: center;
      list-style: none;
      background: var(--background);
      background-size: contain;
  }

      li {
          position: relative;
          height: 100%;
  }

  li[aria-current='page']::before {
      --size: 6px;
      content: '';
      width: 0;
      height: 0;
      position: absolute;
      top: 0;
      left: calc(50% - var(--size));
      border: var(--size) solid transparent;
      border-top: var(--size) solid var(--color-theme-1);
  }
</style>