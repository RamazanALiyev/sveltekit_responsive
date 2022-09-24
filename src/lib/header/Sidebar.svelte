<script>
	import { fly } from 'svelte/transition';
	export let show = true;
</script>

{#if show}
	<div
		transition:fly={{ x: 400, opacity: 1 }}
		class="fixed right-0 left-0 bottom-0 h-[91vh] bg-white"
	>
		<ul class="mt-4">
			<li class="py-2 pl-5 text-black text-3xl font-medium workSans hover:bg-emerald-400 hover:text-white">Home</li>
			<li class="py-2 pl-5 text-black text-3xl font-medium workSans hover:bg-emerald-400 hover:text-white">
				Portfolio
			</li>
			<li class="py-2 pl-5 text-black text-3xl font-medium workSans hover:bg-emerald-400 hover:text-white">
				Services
			</li>
			<li class="py-2 pl-5 text-black text-3xl font-medium workSans hover:bg-emerald-400 hover:text-white">
				<a href="/contact">Contact</a>
			</li>
		</ul>
	</div>
{/if}

<style>
	@import url('https://fonts.googleapis.com/css2?family=Work+Sans:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

	li.workSans {
		font-family: 'Work Sans', sans-serif;
	}
</style>
