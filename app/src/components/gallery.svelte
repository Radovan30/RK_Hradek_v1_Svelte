<script>
	import img1 from '../img/upload/2017_01.webp';
	import img2 from '../img/upload/2017_02.webp';
	import img3 from '../img/upload/2017_03.webp';
	import img4 from '../img/upload/2017_04.webp';
	import img5 from '../img/upload/2017_05.webp';
	import img6 from '../img/upload/2017_06.webp';

	let years = 2017;


</script>

<article id="gallery" class="container mx-auto px-5 py-2 lg:px-30 lg:pt-4 mb-6">
	<section>
		<div>
			<h1 class="text-xl font-bold text-center mt-4 mb-6">ROČNÍK {years}</h1>
		</div>
	</section>

	<section class="-m-1 flex flex-wrap md:-m-2">
		<div class="flex w-1/2 flex-wrap">
			<div class="w-1/2 p-1 md:p-2">
				<img
					alt="gallery"
					class="block h-full w-full rounded-lg object-cover object-center hover:scale-105"
					src={img2}
				/>
			</div>
			<div class="w-1/2 p-1 md:p-2">
				<img
					alt="gallery"
					class="block h-full w-full rounded-lg object-cover object-center hover:scale-105"
					src={img3}
				/>
			</div>
			<div class="w-full p-1 md:p-2">
				<img
					alt="gallery"
					class="block h-full w-full rounded-lg object-cover object-center hover:scale-105"
					src={img1}
				/>
			</div>
		</div>
		<div class="flex w-1/2 flex-wrap">
			<div class="w-full p-1 md:p-2">
				<img
					alt="gallery"
					class="block h-full w-full rounded-lg object-cover object-center hover:scale-105"
					src={img5}
				/>
			</div>
			<div class="w-1/2 p-1 md:p-2">
				<img
					alt="gallery"
					class="block h-full w-full rounded-lg object-cover object-center hover:scale-105"
					src={img4}
				/>
			</div>
			<div class="w-1/2 p-1 md:p-2">
				<img
					alt="gallery"
					class="block h-full w-full rounded-lg object-cover object-center hover:scale-105"
					src={img6}
				/>
			</div>
		</div>
	</section>
</article>

<style>
</style>
