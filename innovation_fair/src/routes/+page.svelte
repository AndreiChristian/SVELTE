<script>
	import Hero from '../Hero.svelte';
	import Opporunities from '../Opporunities.svelte';
	import Speakers from '../Speakers.svelte';
</script>

<Hero />
<Opporunities />
<Speakers />

<style lang="postcss">
	:global(html) {
		font-family: 'Ysabeau', sans-serif;
		background-color: theme(colors.gray.50);
	}
</style>
