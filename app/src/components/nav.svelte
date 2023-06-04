<script>
	import Logo from '../img/logo_rkhradek.webp';
	import Hamburger from './navBurger.svelte';
	import Contact from './contact.svelte';
</script>

<nav class="bg-gray-50">
	<div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
		<a href={Logo} class="flex items-center">
			<img src={Logo} class="h-12" alt="logo" />
		</a>

		<Hamburger />

		<div class="hidden w-full md:block md:w-auto text-center">
			<ul
				class="flex flex-col font-medium mt-4 rounded-lg bg-gray-50 md:flex-row md:space-x-8 md:mt-0 md:border-0 md:bg-transparent"
			>
				<li>
					<a
						href="#onas"
						class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100
						hover:text-amber-500
						md:hover:bg-transparent md:border-0 md:hover:text-amber-500 md:p-0 md:hover:border-t-2 border-gray-500"
						>O nás</a
					>
				</li>
				<li>
					<a
						href="#gallery"
						class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100
						hover:text-amber-500 md:hover:bg-transparent md:border-0 md:hover:text-amber-500 md:p-0 md:hover:border-t-2 border-gray-500"
						>Alvaréz</a
					>
				</li>
				<li>
					<Contact />
				</li>
			</ul>
		</div>
	</div>
</nav>

<style>
</style>
