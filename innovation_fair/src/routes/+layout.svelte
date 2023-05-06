<script>
	import ProgressBar from '../ProgressBar.svelte';
	import '../app.css';
</script>

<!-- <ProgressBar /> -->
<nav>
	<div
		class="flex justify-between items-center fixed top-0 left-0 w-full px-2 py-2 bg-gray-50 shadow-md"
	>
		<span class="text-lg">Beyond Welness</span>

		<svg
			xmlns="http://www.w3.org/2000/svg"
			fill="none"
			viewBox="0 0 24 24"
			stroke-width="1.5"
			stroke="currentColor"
			class="w-6 h-6"
		>
			<path
				stroke-linecap="round"
				stroke-linejoin="round"
				d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
			/>
		</svg>
	</div>
</nav>

<slot />
