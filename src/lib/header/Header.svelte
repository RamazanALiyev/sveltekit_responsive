<script>
	import { page } from '$app/stores';
	import logo from './svelte-logo.svg';
	import GiHamburgerMenu from 'svelte-icons/gi/GiHamburgerMenu.svelte';
	import Sidebar from './Sidebar.svelte';
	let sidebar_show = false;
</script>

<header class="bg-emerald-400 h-[74px] text-white flex items-center border-b">
	<div class="flex justify-between w-[95%] mx-auto items-center md:flex-row md:justify-between md:w-[90%]">
		<div>
			<a class="flex justify-center items-center" href="/">
				<img src={logo} alt="SvelteKit" />
				<span class="ml-2 text-[30px]">Start</span>
			</a>
		</div>
		<div class="w-[20px] h-[20px] sm:block md:hidden">
			<button on:click={() => sidebar_show = !sidebar_show}><GiHamburgerMenu /></button>
		</div>
		<nav class="hidden sm:hidden md:block" data-sveltekit-prefetch>
			<ul class="md:flex">
				<li class="mx-4" class:active={$page.url.pathname === '/'}>
					<a href="/">Home</a>
				</li>
				<li class="mx-4" class:active={$page.url.pathname === '/'}>
					<a href="/">Portfolio</a>
				</li>
				<li class="ml-4" class:active={$page.url.pathname === '/'}>
					<a href="/">Services</a>
				</li>
				<li class="mx-4" class:active={$page.url.pathname === '/'}>
					<a href="/">Contact</a>
				</li>
			</ul>
		</nav>
	</div>

	<Sidebar bind:show={sidebar_show}/>
</header>
