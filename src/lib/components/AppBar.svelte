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
		position: fixed;
		z-index: 50;
		background: rgba(27, 27, 27, 0.43);
		box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
		backdrop-filter: blur(5px);
		-webkit-backdrop-filter: blur(5px);
		width: 100%;
		color: #fff;
	}
</style>
