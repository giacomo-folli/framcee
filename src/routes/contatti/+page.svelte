<script lang="ts">
	import MailIcon from '$lib/components/Icons/MailIcon.svelte';
	import MapsIcon from '$lib/components/Icons/MapsIcon.svelte';
	import PhoneIcon from '$lib/components/Icons/PhoneIcon.svelte';

	let name: string, email: string, message: string;
</script>

<div class="h-[100vh] px-[25px] flex flex-col justify-center">
	<p class="font-bold text-5xl mb-4">Mettiti in contatto</p>
	<p class="text-xl">Hai qualche domanda?</p>
	<p class="text-sm">Per qualsiasi domanda, non esitare a scrivermi.</p>
</div>

<section class="relative px-[25px] py-14 md:py-24">
	<div class="mx-auto flex flex-col md:flex-row justify-between items-center max-w-5xl">
		<div class="flex flex-col gap-6 items-start prose">
			<div>
				<h3 class="">
					<MailIcon />
					Email
				</h3>
				<p class="text-sm underline">
					<a href="mailto:franciberno@test.com"> franciberno@test.com </a>
				</p>
			</div>
			<div>
				<h3 class="">
					<PhoneIcon />
					Telefono
				</h3>
				<p class="text-sm">+39 999 99999</p>
			</div>
			<div>
				<h3 class="">
					<MapsIcon />
					Indirizzo
				</h3>
				<p class="text-sm">Piazza Borsellino e Falcone, Salsomaggiore Terme (PR)</p>
			</div>
		</div>

		<div class="pt-20">
			<iframe
				class="w-[350px] h-[350px] md:w-[600px] md:h-[450px]"
				src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2830.15071341901!2d9.994262475811768!3d44.81849417107069!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4780610fc6baf70f%3A0xeef1cc54b70ac796!2sWeMove%20Personal%20Training%20Center!5e0!3m2!1sit!2sit!4v1719758259704!5m2!1sit!2sit"
				style="border:0;"
				allowfullscreen={true}
				loading="lazy"
				referrerpolicy="no-referrer-when-downgrade"
			></iframe>
		</div>
	</div>
</section>

<section class="relative px-[25px] py-14 md:py-24">
	<div class="mx-auto mb-8">
		<h2 class="text-2xl font-bold text-center">Contattaci</h2>
		<p class="text-center">
			Hai domande? Hai bisogno di richiedere un preventivo? Compila il modulo qui sotto.
		</p>
		<div class="mx-auto divider divider-neutral max-w-2xl"></div>
	</div>

	<div class="mx-auto max-w-xl flex flex-col items-center justify-center gap-6">
		<div class="w-full">
			<label for="name">Nome:</label>
			<input
				class="w-full rounded-none border border-black h-8 mt-1 p-2 text-sm"
				id="name"
				type="text"
				bind:value={name}
				required
			/>
		</div>

		<div class="w-full">
			<label for="email">Email:</label>
			<input
				class="w-full rounded-none border border-black h-8 mt-1 p-2 text-sm"
				id="email"
				type="email"
				bind:value={email}
				required
			/>
		</div>

		<div class="w-full">
			<label for="message">Messaggio:</label>
			<textarea
				class="w-full rounded-none border border-black min-h-32 mt-1 p-2 text-sm"
				id="message"
				bind:value={message}
				required
			></textarea>
		</div>

		<div class="flex items-center gap-2">
			<input id="terms" type="checkbox" class="checkbox checkbox-xs rounded-md" />
			<label for="terms">Accetto i termini e le condizioni</label>
		</div>

		<button class="btn btn-primary bg-black border-none hover:bg-black text-white">Invia</button>
	</div>
</section>

<section class="relative px-[25px] py-14 md:py-24 w-full flex justify-center">
	<div class="join join-vertical w-full max-w-3xl">
		<div class="collapse collapse-arrow join-item border-base-300 border">
			<input type="radio" name="my-accordion-4" />
			<div class="collapse-title text-xl font-medium"># Domanda 1</div>
			<div class="collapse-content">
				<p>Risposta</p>
			</div>
		</div>
		<div class="collapse collapse-arrow join-item border-base-300 border">
			<input type="radio" name="my-accordion-4" />
			<div class="collapse-title text-xl font-medium"># Domanda 2</div>
			<div class="collapse-content">
				<p>Risposta</p>
			</div>
		</div>
		<div class="collapse collapse-arrow join-item border-base-300 border">
			<input type="radio" name="my-accordion-4" />
			<div class="collapse-title text-xl font-medium"># Domanda 3</div>
			<div class="collapse-content">
				<p>Risposta</p>
			</div>
		</div>
	</div>
</section>
