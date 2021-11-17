<nav>
	<ul>
		<li><a href="/">Home</a></li>
		<li><a href="/oldFetch">Old Fetch</a></li>
		<li><a href="/newFetch">New Fetch</a></li>
	</ul>
</nav>

<slot />

<style>
	ul {
		display: flex;
		padding: 0px;
		margin: 0px;
		list-style: none;
	}

	li {
		margin-right: 20px;
		color: #555;
	}
	a {
		text-decoration: none;
	}
</style>
