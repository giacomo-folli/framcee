<script lang="ts">
	import ChevronDown from '../Icons/ChevronDown.svelte';

	export let open: boolean = false;
</script>

<div class="text-black bg-white">
	<nav>
		<div class="w-full flex items-center p-3 justify-between">
			<div class="flex items-center gap-4">
				<div class="font-bold text-2xl bg-black text-white p-1 px-3">
					<a href="/"> F </a>
				</div>

				<a href="/storia">La mia storia</a>
				<a href="/servizi">Servizi</a>
				<a href="/contatti">Contatti</a>
				<!-- <button class="flex items-baseline gap-[3px]"
					>Altro
					<ChevronDown className="size-3" />
				</button> -->
			</div>

			<div>
				<button
					class="transition border border-black hover:bg-black hover:text-white rounded-sm px-4 py-1.5"
				>
					Prossime sessioni
				</button>
			</div>
		</div>
	</nav>
	<div class="w-full border-b border-black" />
</div>
