<script lang="ts">
	export let open: boolean = false;
</script>

<div class="text-black bg-white">
	<nav>
		<div class="w-full flex items-center p-2 justify-between">
			<div class="flex items-center gap-4">
				<div class="font-bold text-2xl bg-black text-white p-1 px-3.5">
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

			<div class="flex gap-4">
				<button
					class="btn btn-sm btn-ghost bg-black text-white hover:bg-black rounded-sm py-none h-fit hidden md:block"
				>
					Prossime sessioni
				</button>
			</div>
		</div>
	</nav>
	<div class="w-full border-b border-black" />
</div>
