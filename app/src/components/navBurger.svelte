<script>
	import NavBurger from '../lib/hamburger.svelte';
    import Contact from './contact.svelte';

	export let open = false;

	export let onClick = () => {
		open = !open;
	};
</script>

<div class="hidden max-md:inline-flex">
	<NavBurger {open} {onClick} />
</div>

{#if open}
<div class="w-full md:block md:w-auto text-center">
		<ul
			class="flex flex-col font-medium mt-4 rounded-lg bg-gray-50 md:flex-row md:space-x-8 md:mt-0 md:border-0 md:bg-transparent"
		>
			<li>
				<a
					href="/"
					class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100
					hover:text-amber-500
					md:hover:bg-transparent md:border-0 md:hover:text-amber-500 md:p-0">O nás</a
				>
			</li>

			<li>
				<a
					href="/"
					class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100
					hover:text-amber-500 md:hover:bg-transparent md:border-0 md:hover:text-amber-500 md:p-0">Alvaréz</a
				>
			</li>
			<li>
				<Contact/>
			</li>
		</ul>
	</div>
{/if}

<style>
</style>
