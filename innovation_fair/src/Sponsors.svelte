<script>
	const sponsors = [
		{
			id: 1,
			name: 'Four Seasons',
			url: 'https://www.fourseasons.com/geneva/offers/?ppc=true&utm_source=google&utm_medium=paidsearch&utm_campaign=acronym-gen-hre-low-allglobalbrand-na&utm_content=na-71700000101050344-58700008259506371-0&utm_term=na&gad=1&gclid=Cj0KCQjw0tKiBhC6ARIsAAOXutmgcQp0MtxItjP5bMugvr4bgCGPqDr1oP0xFo4BVaM7KLmoyyenXCQaAqKZEALw_wcB&gclsrc=aw.ds'
		},
		{
			id: 2,
			name: 'La Moderne',
			url: 'https://www.lemoderne.ch/'
		}
	];
</script>

<div class=" bg-img flex flex-col justify-around items-center h-screen text-center box-border">
	<h1 class="text-center text-cyan-950 text-xl">
		Our <span style="font-family: 'Meddon', cursive;" class="text-amber-500 text-2xl">Sponsors</span
		>
	</h1>
	{#each sponsors as sponsor}
		<div class="flex flex-col justify-center items-center">
			<a target="_blank" href={sponsor.url}>
				<img class=" w-48" src={`./sponsors/${sponsor.id}.png`} alt={sponsor.name} /></a
			>
			<!-- <span class="text-cyan-800 text-3xl">{sponsor.name}</span> -->
		</div>
	{/each}

	<p class="  text-cyan-950 italic">Willing to become a sponsor? Get in touch!</p>
</div>
