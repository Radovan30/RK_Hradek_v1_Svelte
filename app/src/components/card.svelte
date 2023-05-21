<script>
	import Img1 from '../img/upload/2018_08.webp';
	import Img2 from '../img/upload/2021_02.webp';
	import Img3 from '../img/upload/2021_03.webp';
</script>

<div class="absolute mt-5 z-1">
	<svg
		id="visual"
		viewBox="0 0 1600 1380"
		width="1600"
		height="1380"
		xmlns="http://www.w3.org/2000/svg"
		xmlns:xlink="http://www.w3.org/1999/xlink"
		version="1.1"
		><path
			d="M674 0L660.8 35.2C647.7 70.3 621.3 140.7 592.8 211.2C564.3 281.7 533.7 352.3 533.2 422.8C532.7 493.3 562.3 563.7 586.2 634.2C610 704.7 628 775.3 645.2 845.8C662.3 916.3 678.7 986.7 688.5 1057.2C698.3 1127.7 701.7 1198.3 692.5 1268.8C683.3 1339.3 661.7 1409.7 650.8 1444.8L640 1480L0 1480L0 1444.8C0 1409.7 0 1339.3 0 1268.8C0 1198.3 0 1127.7 0 1057.2C0 986.7 0 916.3 0 845.8C0 775.3 0 704.7 0 634.2C0 563.7 0 493.3 0 422.8C0 352.3 0 281.7 0 211.2C0 140.7 0 70.3 0 35.2L0 0Z"
			fill="#fed7aa"
			stroke-linecap="round"
			stroke-linejoin="miter"
		/></svg
	>
</div>

<article class="grid justify-items-center">
	<section class="mt-10 z-10">
		<a
			href={Img1}
			class="flex flex-col items-center bg-white border border-gray-200 rounded-lg shadow md:flex-row md:max-w-xl hover:bg-gray-100 dark:border-gray-700 dark:bg-gray-800 dark:hover:bg-gray-700"
		>
			<div class="flex flex-col justify-between p-4 leading-normal">
				<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
					Kdo jsme?
				</h5>
				<p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
					Jsme otec a tři děti, kteří mají rádi čas strávený v přírodě s lidmi, kteří se rádi baví a
					jen tak se něčeho nebojí.
				</p>
			</div>
			<img
				class="object-cover w-full rounded-t-lg h-56 md:h-auto md:w-48 md:rounded-none md:rounded-r-lg"
				src={Img1}
				alt=""
			/>
		</a>
	</section>
	<section class="mt-10 z-10">
		<a
			href={Img2}
			class="flex flex-col items-center bg-white border border-gray-200 rounded-lg shadow md:flex-row md:max-w-xl hover:bg-gray-100 dark:border-gray-700 dark:bg-gray-800 dark:hover:bg-gray-700"
		>
			<div class="flex flex-col justify-between p-4 leading-normal">
				<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
					Co děláme?
				</h5>
				<p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
					Každoročně v srpnu organizujeme tábor, který začíná ve čtvrtek a končí v neděli. Na tento
					tábor jsou zváni pouze tatínkové s dětmi. V rámci tábora je vždy akce, na kterou jsou
					maminky i široká veřejnost zvány.
				</p>
			</div>
			<img
				class="object-cover w-full rounded-t-lg h-56 md:h-auto md:w-48 md:rounded-none md:rounded-r-lg"
				src={Img2}
				alt=""
			/>
		</a>
		<section />
		<section class="mt-10 z-10">
			<a
				href={Img3}
				class="flex flex-col items-center bg-white border border-gray-200 rounded-lg shadow md:flex-row md:max-w-xl hover:bg-gray-100 dark:border-gray-700 dark:bg-gray-800 dark:hover:bg-gray-700"
			>
				<div class="flex flex-col justify-between p-4 leading-normal">
					<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
						Proč je tábor určen pouze pro otce a děti?
					</h5>
					<p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
						Protože věříme, že čas strávený s tátou v přírodě, kdy se můžeme i zašpinit, dozvědět se
						něco o přírodě a být se skvělou partou je velice obohacující. A také proto aby maminky
						měly na nějakou chvíli čas pro sebe.
					</p>
				</div>
				<img
					class="object-cover w-full rounded-t-lg h-56 md:h-auto md:w-48 md:rounded-none md:rounded-r-lg"
					src={Img3}
					alt=""
				/>
			</a>
			<section />
		</section>
	</section>
</article>

<style>
</style>
