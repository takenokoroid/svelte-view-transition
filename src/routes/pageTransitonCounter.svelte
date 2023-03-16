<script lang="ts">
	import { pageTransition } from '$lib/transition';

	let count = 0;
	const increment = () => {
		count++;
	};
</script>

<div class="content">{count}</div>
<button on:click={() => pageTransition(increment)}>increment</button>

<style>
	.content {
		font-size: 36pt;
	}
</style>
