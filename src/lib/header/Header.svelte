<script>
	import { page } from '$app/stores';
	import logo from './svelte-logo.svg';
</script>

<header class="h-[200px] bg-black text-white flex justify-between">
	<div class="corner">
		<a href="/">
			<img src={logo} alt="SvelteKit" />
		</a>
	</div>
	<nav data-sveltekit-prefetch>
		<ul>
			<li class="text-rose-400" class:active={$page.url.pathname === '/'}>
				<a href="/">Home</a>
			</li>
			<li class:active={$page.url.pathname === '/about'}>
				<a href="/about">About</a>
			</li>
			<li class:active={$page.url.pathname === '/todos'}>
				<a href="/todos">Todos</a>
			</li>
		</ul>
	</nav>
</header>