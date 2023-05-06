<script>
	import { onMount, onDestroy } from 'svelte';

	let scrollPercentage = 0;

	const calculateScrollPercentage = () => {
		const scrollTop = window.scrollY;
		const windowHeight = window.innerHeight;
		const docHeight = document.documentElement.scrollHeight;
		const totalDocScrollLength = docHeight - windowHeight;
		scrollPercentage = (scrollTop / totalDocScrollLength) * 100;
	};

	onMount(() => {
		window.addEventListener('scroll', calculateScrollPercentage);
	});

	onDestroy(() => {
		window.removeEventListener('scroll', calculateScrollPercentage);
	});
</script>

<div class="progress-container">
	<div class="progress-bar bg-cyan-800" style="width: {scrollPercentage}%;" />
</div>

<style>
	.progress-container {
		width: 100%;
		box-sizing: border-box;
		height: 5px;
		position: fixed;
		top: 0;
		left: 0;
		z-index: 100;
	}

	.progress-bar {
		height: 100%;
		transition: width 0.1s;
	}
</style>
