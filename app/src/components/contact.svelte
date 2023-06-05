<script>
	import Modal from '../lib/modal.svelte';

	const facebook = 'https://www.facebook.com/alvarezhradek';
	const telephone = 724096832;
	const email = 'dandysz@seznam.cz';

	let showModal = false;
</script>

<a
	on:click={() => (showModal = true)}
	href="/"
	class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100
						hover:text-amber-500 md:hover:bg-transparent md:border-0 md:hover:text-amber-500 md:p-0"
	>Kontakt</a
>

<Modal bind:showModal>
	<h1 slot="header">KONTAKT</h1>

	<form class="definition-list" name="msgContact">
		<label for="message" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"
			>Napište nám

			<input
				id="name"
				name="username"
				type="text"
				class="block p-1 w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300
				focus:outline-none focus:border-red-400 focus:ring-red-400 focus:ring-1"
				placeholder="Vaše jméno*"
			/>
			<input
				id="email"
				type="email"
				name="email"
				class="block p-1 w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300
				focus:outline-none focus:border-red-400 focus:ring-red-400 focus:ring-1"
				placeholder="Váš email*"
			/>

			<textarea
				id="message"
				name="message"
				rows="4"
				class="block p-2 w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300
				focus:outline-none focus:border-red-400 focus:ring-red-400 focus:ring-1"
				placeholder="Zde piště zprávu..."
			/>

			<input
				type="button"
				class="rounded-md bg-gray-50 border border-gray-300  hover:bg-sky-600 hover:text-white p-1 focus:ring-2 focus:ring-offset-2 focus:ring-sky-500 focus:outline-none rounded-full"
				value="Odeslat"
			/>
		</label>
	</form>

	<div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-6">
		<section class="flex items-center gap-x-8">
			<a
				aria-label="facebook"
				href={facebook}
				class="focus:ring-2 focus:ring-offset-2 focus:ring-sky-600 focus:outline-none rounded-full"
			>
				<svg
					class="fill-current text-gray-500 dark:text-white hover:text-sky-700"
					width="32"
					height="32"
					viewBox="0 0 22 22"
					fill="none"
					xmlns="http://www.w3.org/2000/svg"
				>
					<path
						fill-rule="evenodd"
						clip-rule="evenodd"
						d="M21.5 11.0631C21.5 5.26467 16.7984 0.56311 11 0.56311C5.20156 0.56311 0.5 5.26467 0.5 11.0631C0.5 16.3037 4.33906 20.6476 9.35938 21.4361V14.0992H6.69266V11.0631H9.35938V8.74983C9.35938 6.11873 10.9273 4.6642 13.3255 4.6642C14.4744 4.6642 15.6763 4.86952 15.6763 4.86952V7.45373H14.3516C13.048 7.45373 12.6402 8.2628 12.6402 9.09436V11.0631H15.552L15.087 14.0992H12.6406V21.437C17.6609 20.649 21.5 16.3051 21.5 11.0631Z"
						fill="currentColor"
					/>
				</svg>
			</a>
			<a
				href="tel: {telephone}"
				aria-label="phone"
				class="focus:ring-2 focus:ring-offset-2 focus:ring-teal-600 focus:outline-none rounded-full"
			>
				<svg
					class="fill-current text-gray-500 dark:text-white hover:text-teal-700"
					width="32"
					height="32"
					viewBox="0 0 24 24"
					fill="none"
					xmlns="http://www.w3.org/2000/svg"
				>
					<path
						d="M12 0c-6.627 0-12 5.373-12 12s5.373 12 12 12 12-5.373 12-12-5.373-12-12-12zm3.445 17.827c-3.684 1.684-9.401-9.43-5.8-11.308l1.053-.519 1.746 3.409-1.042.513c-1.095.587 1.185 5.04 2.305 4.497l1.032-.505 1.76 3.397-1.054.516z"
						fill="currentColor"
					/>
					<path
						d="M12 0C5.3736 0 0 5.3736 0 12C0 18.6264 5.3736 24 12 24C18.6264 24 24 18.6264 24 12C24 5.3736 18.6264 0 12 0ZM18.8491 14.8409C18.8157 15.5744 18.6991 16.0752 18.5288 16.5135C18.1708 17.4391 17.4391 18.1708 16.5135 18.5288C16.0754 18.6991 15.5744 18.8156 14.8411 18.8491C14.1063 18.8826 13.8715 18.8906 12.0002 18.8906C10.1287 18.8906 9.8941 18.8826 9.15912 18.8491C8.42578 18.8156 7.9248 18.6991 7.48663 18.5288C7.02667 18.3558 6.61029 18.0846 6.26605 17.7339C5.91559 17.3899 5.64441 16.9733 5.47137 16.5135C5.30109 16.0754 5.18445 15.5744 5.15112 14.8411C5.11725 14.1061 5.10938 13.8713 5.10938 12C5.10938 10.1287 5.11725 9.89392 5.15094 9.15912C5.18427 8.4256 5.30072 7.9248 5.47101 7.48645C5.64404 7.02667 5.91541 6.61011 6.26605 6.26605C6.61011 5.91541 7.02667 5.64423 7.48645 5.47119C7.9248 5.3009 8.4256 5.18445 9.15912 5.15094C9.89392 5.11743 10.1287 5.10938 12 5.10938C13.8713 5.10938 14.1061 5.11743 14.8409 5.15112C15.5744 5.18445 16.0752 5.3009 16.5135 5.47101C16.9733 5.64404 17.3899 5.91541 17.7341 6.26605C18.0846 6.61029 18.356 7.02667 18.5288 7.48645C18.6993 7.9248 18.8157 8.4256 18.8492 9.15912C18.8828 9.89392 18.8906 10.1287 18.8906 12C18.8906 13.8713 18.8828 14.1061 18.8491 14.8409Z"
						fill="currentColor"
					/>
				</svg>
			</a>
			<a
				href="mailto: {email}"
				aria-label="mailto"
				class="focus:ring-2 focus:ring-offset-2 focus:ring-amber-400 focus:outline-none rounded-full"
			>
				<svg
					class="fill-current text-gray-500 dark:text-white hover:text-amber-500"
					width="32"
					height="32"
					viewBox="0 0 24 24"
					fill="none"
					xmlns="http://www.w3.org/2000/svg"
				>
					<path
						d="M12 .02c-6.627 0-12 5.373-12 12s5.373 12 12 12 12-5.373 12-12-5.373-12-12-12zm6.99 6.98l-6.99 5.666-6.991-5.666h13.981zm.01 10h-14v-8.505l7 5.673 7-5.672v8.504z"
						fill="currentColor"
					/>
				</svg>
			</a>
		</section>
	</div>
</Modal>

<style>
	input,
	label,
	textarea {
		margin-top: 10px;
	}
</style>
