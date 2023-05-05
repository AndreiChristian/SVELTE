<script>
	let opportunities = [
		{
			title: 'Wellness Tech Showcase',
			body: 'Discover cutting-edge wellness technologies and solutions from leading companies.'
		},
		{
			title: 'Expert Panel Discussions',
			body: 'Join panel discussions featuring industry experts discussing the latest trends and innovations in wellness.'
		},
		{
			title: 'Workshops',
			body: 'Participate in hands-on workshops to learn new skills and techniques to improve your wellness journey.'
		},
		{
			title: 'Networking',
			body: 'Connect with like-minded individuals, professionals, and organizations to grow your network in the wellness industry.'
		}
	];
</script>

<div class=" bg-img flex flex-col justify-around items-center h-screen text-center box-border">
	<h1 class="text-center text-cyan-950 text-xl">
		An <span style="font-family: 'Meddon', cursive;" class="text-amber-500 text-2xl"
			>Opportunity</span
		> not to miss
	</h1>
	{#each opportunities as o}
		<div class=" shadow-lg rounded-xl w-5/6 p-6 border-t-4 border-opacity-70">
			<h1 class=" text-cyan-950 text-xl">{o.title}</h1>
			<p>{o.body}</p>
		</div>
	{/each}
</div>
