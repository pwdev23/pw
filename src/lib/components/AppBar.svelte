<script>
</script>

<header class="app-bar-surface">
	<div
		class="text-small"
		style="text-align: center; background-color: var(--secondary-color); padding: 0.25rem;"
	>
		In development
	</div>
	<slot />
</header>

<style>
	.app-bar-surface {
		position: sticky;
		z-index: 50;
		background: var(--text-color);
		width: 100%;
		color: #fff;
	}
</style>
