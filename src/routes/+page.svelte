<script lang="ts">
	import Armonica from '$lib/components/common/Armonica.svelte';
	import Card from '$lib/components/common/Card.svelte';
</script>

<section class="relative">
	<div class="flex flex-col lg:flex-row justify-center items-center min-h-[100vh] pt-4 pb-4">
		<div id="slogan" class="text-center text-[12vw] lg:text-[5vw] font-semibold leading-tight">
			“Ritorna in controllo <br /> del tuo corpo”
		</div>
	</div>
</section>

<section class="relative px-[18px] py-14 md:pt-24">
	<section class="light lg:pb-0 bg-white text-zinc-900">
		<div class="container px-4">
			<div class="grid grid-cols-12 md:gap-8">
				<div class="col-span-12 lg:col-span-6">
					<div class="flex justify-center items-center relative h-[500px]">
						<img src="/logo.png" class="max-w-full h-[500px] rounded-xl" alt="aa" />
					</div>
				</div>
				<div class="col-span-12 lg:col-span-6 flex flex-col justify-center">
					<div>
						<h3 class="text-2xl md:text-base">Chi sono</h3>
						<h2 class="text-2xl font-bold leading-none md:text-5xl md:leading-none mb-6">
							Francesco, la mia storia
						</h2>
						<p
							class="text-base sm:text-lg leading-relaxed tracking-wide break-words mt-4 md:mt-12 opacity-75"
						>
							I am a website designer from Lousiana, with a strong focus in UI/UX design. I love to
							get new experiences and always learn from my surroundings. I've done more than 285
							projects. You can check it through portfolio section on this website. I looking
							forward to any opportunities and challenges. Ex velit cupidatat magna voluptate
							deserunt quis et dolor adipisicing elit culpa ad exercitation proident irure deserunt
							irure. I look forward to any opportunities and challenges.
						</p>
						<div class="grid grid-cols-12">
							<div class="col-span-12 lg:col-span-4">
								<button
									class="py-3 px-7 text-white bg-blue-600 hover:text-white hover:bg-opacity-90 mt-12 w-full rounded-md"
								>
									Read More
								</button>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>
</section>

<section class="px-[18px] mt-4 mb-20">
	<h2 class="text-lg text-center font-bold leading-none md:text-3xl md:leading-none mt-6 mb-8">
		Il mio percorso
	</h2>

	<div class="mx-auto max-w-2xl">
		<Armonica />
	</div>
</section>

<section class="relative mt-8">
	<div class="w-full">
		<img src="/homepage.jpg" alt="aaa" class="object-cover w-full h-[500px] filter brightness-75" />
	</div>

	<div class="absolute top-0 bottom-0 flex flex-col justify-center max-w-lg p-4 pl-8">
		<p class="text-lg text-white">Il mio metodo, la mia passione</p>
		<p class="text-2xl text-white font-semibold">
			L‘armonia dei nostri movimenti, l’equilibrio delle nostre azioni sul tappetino e quindi il
			controllo di gesti e parole nella vita quotidiana
		</p>
	</div>
</section>

<section class="px-[18px] py-14 md:py-24 bg-white dark:bg-[#0b1727] text-zinc-900 dark:text-white">
	<h1 class="text-3xl font-semibold md:text-[35px] mb-4 text-nowrap">Metodo di allenamento</h1>
	<div class="container px-4 mx-auto">
		<!-- heading -->
		<div class="flex gap-6 max-w-7xl mt-4">
			<div class="basis-1/2 text-center lg:text-start">
				<div class="h-full flex flex-col items-center justify-center text-center">
					<div class="flex justify-center items-center w-full gap-8">
						<!-- card starts -->
						<div class="basis-1/2 mb-8 text-center">
							<Card />
						</div>
						<!-- card ends -->
						<!-- card starts -->
						<div class="basis-1/2 mb-8 text-center">
							<Card />
						</div>
						<!-- card ends -->
					</div>
					<div class="flex justify-center items-center w-full gap-8">
						<!-- card starts -->
						<div class="basis-1/2 text-center">
							<Card />
						</div>
						<!-- card ends -->
						<!-- card starts -->
						<div class="basis-1/2 text-center">
							<Card />
						</div>
						<!-- card ends -->
					</div>
				</div>
			</div>
			<div class="basis-1/2 flex flex-col justify-center">
				<div class="w-full">
					<img src="/homepage.jpg" alt="" class="w-full h-[500px] object-cover rounded-xl" />
				</div>
			</div>
		</div>
	</div>
</section>

<style>
	.fade-on-scroll {
		animation: fade-on-scroll linear both;
		animation-timeline: view();
		animation-range: entry 0% contain 20%;
	}

	@keyframes fade-on-scroll {
		0% {
			opacity: 0;
			transform: translate(0, 40px);
		}
		100% {
			opacity: 1;
			transform: translate(0, 0);
		}
	}
</style>
