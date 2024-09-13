<script lang="ts">
	import { goto } from '$app/navigation';
	import Avatars from '$lib/components/common/Avatars.svelte';
	import Feature from '$lib/components/common/Feature.svelte';
	import TextAndImage from '$lib/components/common/TextAndImage.svelte';
</script>

<section id="hero-section">
	<div
		class="mx-auto max-w-3xl text-center flex flex-col gap-6 justify-center items-center min-h-[100vh]"
	>
		<div>
			<p class="font-semibold text-lg tracking-wide">Libera il tuo potenziale con</p>
			<h1 id="slogan" class="font-bold text-5xl">Francesco Bernini</h1>
		</div>

		<p class="px-10">
			Sperimenta un programma di allenamento trasformativo che si concentra su mobilità, forza,
			flessibilità e coordinazione. Unisciti a Francesco Bernini per raggiungere nuovi limiti.
		</p>

		<div class="flex justify-center items-center gap-4">
			<button class="btn btn-sm rounded-sm bg-white hover:bg-white border-black"
				>Scoprio di più</button
			>
			<button class="btn btn-sm rounded-sm bg-black hover:bg-black text-white"
				>Prenota una lezione grautita</button
			>
		</div>
	</div>
</section>

<section id="image-section">
	<div class="w-full lg:my-8 px-4 md:px-20 lg:max-h-[80vh] overflow-hidden">
		<img width="100%" src="/homepage.jpg" alt="foto" class="object-bottom shadow-xl rounded-md" />
	</div>
</section>

<TextAndImage src="/homepage.jpg" alt="foto" reversed={true}>
	<div slot="text">
		<p class="font-bold text-4xl max-w-xl">
			Libera il tuo potenziale grazie ad un approccio olistico
		</p>
		<p class="text-lg max-w-xl mb-6">
			Credo che la vera forza derivi dalla cura della mente e del corpo. Con la mia esperienza in
			mobilità, forza, flessibilità e coordinazione, ti guiderò verso il raggiungimento dei tuoi
			obiettivi.
		</p>
	</div>
</TextAndImage>

<section id="net-section" class="pt-14 md:pt-28 pb-6 md:pb-20">
	<h2 class="text-center font-bold text-4xl mb-6 md:mb-20">Ho collaborato con</h2>
	<div>
		<Avatars />
	</div>
</section>

<section id="features-section" class="px-[18px]">
	<div class="mt-20 md:mt-32 mb-10 mx-auto flex flex-col items-center">
		<div class="w-full text-pretty md:text-center text-4xl font-bold mb-10">
			Impara a sfruttare il 100% del tuo corpo
		</div>
		<div class="mx-auto p-8 flex flex-col md:flex-row justify-center gap-4">
			<Feature />
		</div>
	</div>
</section>

<TextAndImage src="/homepage.jpg" alt="foto" reversed>
	<div slot="text">
		<div class="basis-1/2 w-full flex flex-col gap-4 justify-center max-w-lg">
			<div class="mb-2">
				<p class="font-semibold text-sm py-3">Trasformazione</p>
				<p class="p-normal">
					Experience a holistic approach to training that focuses on developing your mind and body.
					With Francesco, you'll improve your mobility, strength, flexibility, and coordination,
					leading to overall growth and well-being.
				</p>
			</div>

			<div class="flex flex-col gap-3">
				<div>
					<h5 class="font-semibold">Approccio olistico</h5>
					<p class="p-normal">
						Ricevi un'attenzione e una guida personalizzate per raggiungere i tuoi obiettivi di
						fitness in modo efficace.
					</p>
				</div>
				<div>
					<h5 class="font-semibold">Programmi personalizzati</h5>
					<p class="p-normal">
						Sviluppa la tua mente e il tuo corpo attraverso programmi di allenamento personalizzati
						in base alle tue esigenze.
					</p>
				</div>
			</div>
		</div>
	</div>
</TextAndImage>

<section class="py-16 w-full flex justify-center">
	<button
		on:click={() => goto('/servizi')}
		class="btn btn-primary bg-info-content border-none text-white"
		>Scopri tutti i servizi che offro!
	</button>
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
