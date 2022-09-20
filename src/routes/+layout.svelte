<script>
	import Header from '$lib/header/Header.svelte';
	import '../app.css';
</script>

<Header />

<main class="">
	<slot />
</main>

<footer class="h-[100px] bg-black text-white flex justify-center items-center">
	<p>Footer</p>
</footer>