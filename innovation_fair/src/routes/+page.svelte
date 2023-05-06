<script>
	import Footer from '../Footer.svelte';
import Hero from '../Hero.svelte';
	import Opporunities from '../Opporunities.svelte';
	import Speakers from '../Speakers.svelte';
	import Sponsors from '../Sponsors.svelte';
	import Timetable from '../Timetable.svelte';
</script>

<Hero />
<Opporunities />
<Speakers />
<Timetable />
<Sponsors />
<Footer/>

<style lang="postcss">
	:global(html) {
		font-family: 'Ysabeau', sans-serif;
		background-color: theme(colors.gray.50);
	}
</style>
