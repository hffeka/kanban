<script>
	let workspaces = [
		{ name: '1.', location: '/workspaces/1' },
		{ name: '2.', location: '/workspaces/2' },
		{ name: '3.', location: '/workspaces/3' }
	];
</script>

<h3>your workspaces</h3>

<div class="workspace-list">
	<ul class="workspace-wrapper">
		{#each workspaces as ws}
			<li><a href={ws.location}>{ws.name}</a></li>
		{/each}
	</ul>
</div>

<style>
	.flex-row {
		display: flex;
		align-items: center;
		gap: 2rem;
	}

	.workspace-wrapper > li {
		list-style: none;
	}

	.workspace-wrapper a {
		text-decoration: none;
		color: inherit;
	}
</style>
