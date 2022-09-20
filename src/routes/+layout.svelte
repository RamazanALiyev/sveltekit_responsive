<script>
	// @ts-nocheck

	import Header from '$lib/header/Header.svelte';
	import '../app.css';
	import FaFacebookF from 'svelte-icons/fa/FaFacebookF.svelte';
	import FaInstagram from 'svelte-icons/fa/FaInstagram.svelte';
	import FaTwitter from 'svelte-icons/fa/FaTwitter.svelte';
	import FaPinterestP from 'svelte-icons/fa/FaPinterestP.svelte';
	import FaWhatsapp from 'svelte-icons/fa/FaWhatsapp.svelte';
	import FaYoutube from 'svelte-icons/fa/FaYoutube.svelte';
</script>

<Header/>

<svelte:head>
	<link href="https://unpkg.com/tailwindcss@^1.0/dist/tailwind.min.css" rel="stylesheet"/>
</svelte:head>

<main class="">
	<slot />
</main>

<footer class="bg-emerald-400 h-32 text-white flex items-center border-t">
	<div
		class="flex flex-col justify-center items-center w-[95%] mx-auto md:flex-row md:justify-between md:w-[90%]"
	>
		<div class="flex justify-center items-center w-[80%] h-5 w-full md:w-60">
			<FaFacebookF />
			<FaInstagram />
			<FaTwitter />
			<FaPinterestP />
			<FaWhatsapp />
			<FaYoutube />
		</div>
		<p class="text-xl mt-5 md:mt-0">© Start, 2022. All rights reserved.</p>
	</div>
</footer>
