<script lang="ts"></script>

<section class="relative">
	<div
		class="absolute top-0 left-0 h-full w-full z-[-1] bg-cover bg-no-repeat filter sepia contrast-50"
		style:background-image="url(/homepage.jpg)"
	/>

	<div class="flex flex-col lg:flex-row justify-between min-h-[100vh] pt-20 pb-4">
		<div id="slogan" class="mx-auto p-1 py-14 lg:p-10 lg:mt-8">
			<div class="text-xs lg:text-[1vw] px-6">
				Impara, esplora e conosci te stesso attraverso le pratiche del movimento. 
			</div>

			<div
				class="w-full text-center text-[20vw] lg:text-[10vw] font-semibold leading-none whitespace-pre-wrap"
			>
				PHYSICAL
			</div>
			<div
				class="w-full text-center pt-2 text-[14vw] lg:text-[7vw] tracking-widest lg:tracking-wider leading-[7vw] lg:leading-[4vw] font-semibold whitespace-pre-wrap"
			>
				MOVEMENT
			</div>
			<div
				class="w-full text-center text-[23vw] lg:text-[13vw]  leading-none font-semibold whitespace-pre-wrap"
			>
				GROUPS
			</div>

			<div class="w-full px-6 text-sm lg:text-[2vw] tracking-normal italic">
				Comunità. Supporto. Crescita. Esperienza.
			</div>
		</div>

		<div class="mt-8 flex justify-end lg:p-16">
			<div class="mb-6 mr-2 h-[150px] w-[150px] lg:h-[400px] lg:w-[400px]">
				<img src="/logo.png" alt="log" />
				<div
					class="bg-white bg-opacity-75 px-1 pb-1 text-right underline underline-offset-4 text-[5vw] lg:text-lg tracking-wide lg:tracking-wider lg:text-right"
				>
					<a href="/classi"> prenota ora &rarr; </a>
				</div>
			</div>
		</div>
	</div>
</section>

<section class="relative px-4 border-[18px] border-black">
	<div class="fade-on-scroll absolute top-2 left-2 font-semibold">*Manifesto</div>

	<div class="w-full text-center mt-10 mb-32 lg:mt-20 lg:mb-64 leading-[16vw]">
		<div class="fade-on-scroll text-[25vw] leading-[19vw]">We are</div>
		<div class="fade-on-scroll text-[19vw]">a diverse</div>
		<div class="fade-on-scroll text-[10vw] tracking-tight leading-none text-amber-600 filter sepia-[50%]">group of humans</div>
	</div>

	<div class="ml-[30vw] lg:ml-[70vw] mb-24 lg:mb-48 leading-[8vw]">
		<div class="fade-on-scroll text-[6vw] lg:text-3xl">engaging in many</div>
		<div class="fade-on-scroll text-[6vw] lg:text-3xl tracking-tight italic">types of movement,</div>
	</div>

	<div class="leading-[7vw] tracking-tighter mb-24 lg:mb-64">
		<div class="fade-on-scroll text-[7vw] lg:text-5xl">with the intention of</div>
		<div class="fade-on-scroll text-[7vw] lg:text-5xl font-semibold">learning more about</div>
		<div class="fade-on-scroll text-[15vw] leading-[10vw] italic">ourselves,</div>
	</div>

	<div class="leading-[11vw] mb-32 lg:mb-64">
		<div class="fade-on-scroll text-[12vw] flex gap-2 lg:gap-8">
			both <div class="italic underline underline-offset-8 mt-4 lg:mt-8 text-amber-600 filter sepia-[50%]">physically</div>
		</div>
		<div class="fade-on-scroll text-[13vw] font-[500] flex gap-4 lg:gap-16	">
			and <div class="italic underline underline-offset-8 mt-2 lg:mt-6 text-amber-600 filter sepia-[50%]">mentally</div>
		</div>
	</div>

	<div class="mb-16 lg:mb-32">
		<div class="fade-on-scroll text-[5vw] tracking-tight leading-none italic">
			We are dancers and photographers,
		</div>
		<div class="fade-on-scroll text-[5vw] tracking-wide leading-none text-right font-mono">accountants and managers,</div>
		<div class="fade-on-scroll text-[5vw] leading-none italic font-serif">architects and builders alike.</div>
	</div>

	<div class="leading-[10vw] mb-8 lg:mb-20">
		<div class="fade-on-scroll text-[10vw] tracking-tighter">we are here to learn</div>
		<div class="fade-on-scroll text-[13vw] tracking-tighter flex gap-3 lg:gap-8 items-baseline">and
			<div class="fade-on-scroll lg:text-[16vw] italic text-amber-600 filter sepia-[50%]">
				experience.
			</div>
			</div>
	</div>
</section>

<section class="relative h-96 pt-8 pb-14">
	<div
		class="absolute bg-center top-0 left-0 h-full w-full z-[-1] bg-cover bg-no-repeat filter sepia contrast-50"
		style:background-image="url(/homepage.jpg)"
	/>

	<div
		class="absolute bottom-4 right-4 p-3  filter sepia font-bold shadow-lg border-4 border-black backdrop-blur-sm"
	>
		<button> Unisciti a noi</button>
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