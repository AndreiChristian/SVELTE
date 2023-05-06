<script>
	let speakers = [
		{
			id: 3,
			name: 'Mariana Palmeiro',
			description: 'Wellness & Spa Expert'
		},
		{
			id: 1,
			name: 'Stéphane Reumont',
			description: 'Spa & Welness Director Beau Rivage Lausanne'
		},
		{
			id: 2,
			name: 'Margaux Poilvet',
			description: 'Spa Director Four Seasons Geneva'
		}
	];
</script>

<div class=" bg-img flex flex-col justify-around items-center h-screen text-center box-border">
	<h1 class="text-center text-cyan-950 text-xl">
		Expert <span style="font-family: 'Meddon', cursive;" class="text-amber-500 text-2xl"
			>Speakers</span
		>
	</h1>
	{#each speakers as o}
		<div
			class="flex flex-row items-center justify-center lg:justify-around shadow-lg rounded-xl w-10/12 p-6 border-t-4 border-opacity-70"
		>
			<img
				class="lg:w-1/4 border-b-2 border-amber-500 w-3/5"
				src={`./speakers/${o.id}.png`}
				alt={o.name}
			/>
			<span>
				<h1 class=" text-cyan-950 text-3xl">{o.name}</h1>
				<p>{o.description}</p>
			</span>
		</div>
	{/each}
	<p class="  text-cyan-950 italic">Stay tuned! More to be announced shortly..</p>
</div>
