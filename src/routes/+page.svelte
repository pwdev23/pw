<script>
	import { onMount } from 'svelte';
	import AppBar from '$components/AppBar.svelte';

	onMount(() => {
		const videoElement = document.getElementById('background-video');
		videoElement.play();
	});
</script>

<AppBar>
	<div style="display: flex; align-items: center; padding: 0.5rem 1rem;">
		<img src="logo.png" alt="project-weekend-logo" width="48px" height="48px" />
		<h3 style="color: #fff; margin-left: 1rem;">Project Weekend</h3>
	</div>
</AppBar>
<div />
<div class="container" style="background-color: var(--text-color); color: #fff; height: 100vh;">
	<video class="background-video" id="background-video" autoplay muted loop>
		<source src="video.mp4" type="video/mp4" />
	</video>
	<div
		class="overlay"
		style="height: 100vh; display: flex; flex-direction: column; justify-content: end;"
	>
		<h1 style="color: #fff; padding: 0rem 2rem;">Digital creators</h1>
		<div style="padding: 0rem 2rem;">Build digital product that people loves.</div>
		<div style="padding-bottom: 2rem;" />
	</div>
</div>
<div class="container" style="height: 100vh;">
	<div
		class="overlay"
		style="height: 100vh; display: flex; flex-direction: column; justify-content: end;"
	>
		<h1 style="padding: 0rem 2rem;">Dependably Creative</h1>
		<div style="padding: 0rem 2rem;">
			Our clients choose us for our innovation, and stay for our ability to successfully deliver on
			time and budget. In 15 years and hundreds of challenging projects, we haven’t had one major
			hiccup.
		</div>
		<div style="padding-bottom: 2rem;" />
	</div>
</div>

<style>
	.container {
		position: relative;
		width: 100%;
		display: flex;
		align-items: end;
		flex-direction: column;
		justify-content: end;
	}

	.background-video {
		height: 100%;
		width: 100%;
		object-fit: cover;
	}

	.overlay {
		position: absolute;
		z-index: 10;
		top: 0;
		left: 0;
		width: 100%;
	}
</style>
