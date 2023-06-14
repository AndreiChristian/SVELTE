<script lang="ts">
	import { goto } from '$app/navigation';

	const handleClick = (id: string) => {
		goto(`/product/${id}`);
	};
</script>

<h1>Hello</h1>
<ul>
	<li>
		<button
			on:click={() => {
				handleClick('1');
			}}>1</button
		>
	</li>
	<li>
		<button
			on:click={() => {
				handleClick('2');
			}}>2</button
		>
	</li>
	<li>
		<button
			on:click={() => {
				handleClick('3');
			}}>3</button
		>
	</li>
	<li>
		<button
			on:click={() => {
				handleClick('4');
			}}>4</button
		>
	</li>
	<li>
		<button
			on:click={() => {
				handleClick('5');
			}}>5</button
		>
	</li>
</ul>
