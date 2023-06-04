<script lang="ts">
	import ImgHero from '../img/upload/2020_08.jpg';
</script>

<article
	class="relative overflow-hidden bg-cover bg-no-repeat"
	style="
      background-position: 50%;
      background-image: url('{ImgHero}');
      height: 400px;
    "
>
	<section
		class="absolute bottom-0 left-0 right-0 top-0 h-full w-full overflow-hidden bg-fixed"
		style="background-color: rgba(0, 0, 0, 0.65)"
	>
		<div class="flex h-full items-center justify-center">
			<div class="px-6 text-center md:px-12">
				<h1 id="hero-blink" class="mt-10 text-5xl font-bold">LETNÍ TÁBOR</h1>
				<h3 class="mb-6 text-3xl font-bold">S TATÍNKY</h3>
			</div>
		</div>
	</section>
</article>

<style>
	:root {
		--typewriterSpeed: 5s;
	}

	h1 {
		color: rgba(255, 255, 255, 0.85);
		letter-spacing: 5px;
		animation: typewriter 4s steps(40) 1s 1 normal both,
			blinkTextCursor 500ms steps(40) infinite normal;
	}

	h3 {
		letter-spacing: 5px;
	}

		#hero-blink {
			
			white-space: nowrap;
			overflow: hidden;
			transform: translateY(-50%);
		}

	
		
	@keyframes typewriter {
		from {
			width: 0;
		}
		to {
			width: 580px;
		}
	}

	@keyframes blinkTextCursor {
		from {
			border-right-color: rgba(255, 255, 255, 0.7);
		}
		to {
			border-right-color: transparent;
		}
	}


	h3 {
		color: rgba(255, 255, 255, 0.7);
		opacity: 0;
		transform: translateY(2rem);
		animation: fadeInUp 3s ease calc(var(--typewriterSpeed)) forwards;
	}

	@keyframes fadeInUp {
		to {
			opacity: 1;
			transform: translateY(0);
		}
	}
	@media only screen and (max-width: 600px) {
		h1 {
			font-size: 2rem;
			animation: typewriter 2s steps(40) 1s 1 normal both,
				blinkTextCursor 500ms steps(40) infinite normal;
		}

		@keyframes typewriter {
			from {
				width: 0;
			}
			to {
				width: 400px;
			}
		}
	}

	@media only screen and (max-width: 400px) {
		h1 {
			font-size: 1.5rem;
			animation: typewriter 2s steps(40) 1s 1 normal both,
				blinkTextCursor 500ms steps(40) infinite normal;
		}

		h3 {
			font-size: 1.5rem;
		}

		@keyframes typewriter {
			from {
				width: 0;
			}
			to {
				width: 320px;
			}
		}
	}
</style>
