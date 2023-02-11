<script>
	let name = 'new';
	let isInCreation = false;
	import { page } from '$app/stores';
</script>

<div class="workspace-navigation">
	<h2>workspaces</h2>
	{#if $page.url.pathname == '/workspaces'}
		<a class="look-like-button" href="/workspaces/create">new</a>
	{:else}
		<a class="look-like-button" href="/workspaces">back</a>
	{/if}
</div>

<slot />

<style>
	.workspace-navigation {
		display: flex;
		align-items: center;
		gap: 2rem;
		padding: 0.5rem 1rem;
		height: fit-content;
		border-bottom: 1px solid rgb(202, 202, 202);
	}

	.workspace-navigation > a {
		font-size: 0.9rem;
		color: inherit;
		text-decoration: none;
	}

	h2 {
		font-size: 1.2rem;
	}

	.look-like-button {
		border: 1px solid black;
		border-radius: 0.9rem;
		padding: 0.25rem 0.75rem;
	}

	.look-like-button:hover {
		background-color: black;
		color: white;
	}
</style>
