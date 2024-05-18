<script lang="ts">
	import Card from './Card.svelte';
</script>

<div class="px-[18px] bg-white text-zinc-900">
	<div class="w-full px-4 mx-auto">
		<div class="grid grid-cols-12 gap-6 max-w-7xl mt-4">
			<div class="col-span-12 md:col-span-4 lg:col-span-6 text-center lg:text-start">
				<div class="h-full grid grid-cols-1 lg:grid-cols-2 gap-8 text-center">
					<div class="flex flex-col justify-between w-full">
						<div class="text-center">
							<Card />
						</div>
						<div class="text-center">
							<Card />
						</div>
					</div>
					<div class="flex flex-col justify-between w-full">
						<div class="text-center">
							<Card />
						</div>
						<div class="text-center">
							<Card />
						</div>
					</div>
				</div>
			</div>
			<div class="col-span-12 md:col-span-8 lg:col-span-6 flex flex-col justify-center">
				<div class="w-full">
					<img src="/homepage.jpg" alt="" class="w-full h-[500px] object-cover rounded-xl" />
				</div>
			</div>
		</div>
	</div>
</div>
