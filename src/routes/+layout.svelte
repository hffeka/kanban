<nav class="global-navigation">
	<ul class="navigation-wrapper | no-list-style">
		<li><a class="navigation-link" href="/">home</a></li>
		<li><a class="navigation-link" href="/workspaces">workspaces</a></li>
	</ul>
	<ul class="navigation-wrapper | no-list-style">
		<li><a class="navigation-link" href="/account">account</a></li>
	</ul>
</nav>

<slot />

<style>
	.global-navigation {
		/* border: 1px solid black; */
		display: flex;
		justify-content: space-between;
		padding: 0 1rem;
		border-bottom: 1px solid black;
	}

	.navigation-wrapper {
		/* border: 1px solid black; */
		display: flex;
		gap: 2rem;
		padding: 0;
	}

	.no-list-style {
		/* border: 1px solid black; */
		list-style: none;
	}

	.navigation-link {
		text-decoration: none;
	}
</style>
