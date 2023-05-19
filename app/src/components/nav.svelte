<script>
    import { fly } from 'svelte/transition'
	import Logo from '../img/logo_rkhradek.webp';
	import Hamburger from '../lib/AnimatedHamburger.svelte';

	export let open = false;
	export let onClick = () => {
		open = !open;
	};
</script>

<nav class="border-gray-200 bg-gray-50 dark:bg-gray-800 dark:border-gray-700">
	<div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
		<a href={Logo}>
			<img src={Logo} class="h-14 mr-3" alt="RK Hradek Logo" />
		</a>

		<button
			data-collapse-toggle="navbar-solid-bg"
			type="button"
			class="inline-flex items-center p-2 ml-3 text-sm text-gray-700 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-600 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600 mt-3"
			aria-controls="navbar-solid-bg"
			aria-expanded="false"
		>
			<span class="sr-only">Open main menu</span>
			<svg
				class="w-6 h-6"
				aria-hidden="true"
				fill="currentColor"
				viewBox="0 0 20 20"
				xmlns="http://www.w3.org/2000/svg"
				><path
					fill-rule="evenodd"
					d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z"
					clip-rule="evenodd"
				/></svg
			>
		</button>

		<div class="hidden w-full md:block md:w-auto" id="navbar-solid-bg">
			<ul
				class="flex flex-col font-medium mt-4 rounded-lg bg-gray-50 md:flex-row md:space-x-8 md:mt-0 md:border-0 md:bg-transparent dark:bg-gray-800 md:dark:bg-transparent dark:border-gray-700"
			>
				<li>
					<a
						href="/"
						class="font-bold text-gray-600 block mt-4 lg:inline-block lg:mt-0 hover:text-amber-500"
						aria-current="page">O nás</a
					>
				</li>
				<li>
					<a
						href="/"
						class="font-bold text-gray-600 block mt-4 lg:inline-block lg:mt-0 hover:text-amber-500"
						>Alvaréz</a
					>
				</li>
				<li>
					<a
						href="/"
						class="font-bold text-gray-600 block mt-4 lg:inline-block lg:mt-0 hover:text-amber-500"
						>Kontak</a
					>
				</li>
			</ul>
		</div>
	</div>
</nav>



<navigation class="border-gray-200 bg-gray-50 dark:bg-gray-800 dark:border-gray-700">
	<div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">

		<a href={Logo}>
			<img src={Logo} class="h-14 mr-3" alt="RK Hradek Logo" />
		</a>

<Hamburger {open} {onClick} />
		{#if open}
         <nav transition:fly={{ y: -200, duration: 400 }}>
			<ul
				class="flex flex-col font-medium mt-4 rounded-lg bg-gray-50 md:flex-row md:space-x-8 md:mt-0 md:border-0 md:bg-transparent dark:bg-gray-800 md:dark:bg-transparent dark:border-gray-700"
			>
				<li>
					<a
						href="/"
						class="font-bold text-gray-600 block mt-4 lg:inline-block lg:mt-0 hover:text-amber-500"
						aria-current="page">O nás</a
					>
				</li>
				<li>
					<a
						href="/"
						class="font-bold text-gray-600 block mt-4 lg:inline-block lg:mt-0 hover:text-amber-500"
						>Alvaréz</a
					>
				</li>
				<li>
					<a
						href="/"
						class="font-bold text-gray-600 block mt-4 lg:inline-block lg:mt-0 hover:text-amber-500"
						>Kontak</a
					>
				</li>
			</ul>
            </nav>
		{/if}
	</div>
</navigation>

