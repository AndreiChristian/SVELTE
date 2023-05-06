<script>
	let eventSchedule = [
		{
			time: '14:00 - 14:30',
			title: 'Welcome Drink'
		},
		{
			time: '14:30 - 15:15',
			title: 'Introduction Speaker'
		},
		{
			time: '15:15 - 15:35',
			title: '20 Min Break with Booths'
		},
		{
			time: '15:35 - 16:35',
			title: 'Roundtable'
		},
		{
			time: '16:35 - 17:00',
			title: '20 Min Break with Booths'
		},
		{
			time: '17:00 - 17:45',
			title: 'Keynote Speaker'
		},
		{
			time: '17:45 - 18:05',
			title: '20 Min Break with Booths and Raffle'
		},
		{
			time: '18:15',
			title: 'Auction'
		}
	];
</script>

<div class=" flex flex-col justify-center items-center h-screen box-border">
	<h1 class="text-xl text-cyan-800">
		The <span style="font-family: 'Meddon', cursive;" class="text-amber-500 text-2xl">Schedule</span
		>
	</h1>
	{#each eventSchedule as e}
		<div
			class="flex flex-row items-center justify-between w-9/12 py-3 px-2 border-b-2 border-cyan-800"
		>
			<span class=" text-xl outline-1 outline-neutral-900 text-left w-full">{e.time}</span>
			<span class=" text-xl outline-1 outline-neutral-900 text-left w-full">{e.title}</span>
		</div>
	{/each}
</div>
