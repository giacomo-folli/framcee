<script lang="ts">
	import { slide } from 'svelte/transition';

	let faqs: {
		id: number;
		title: string;
		answer: string;
		active: boolean;
	}[] = [
		{ id: 1, title: 'string', answer: 'string', active: false },
		{ id: 1, title: 'string', answer: 'string', active: false },
		{ id: 1, title: 'string', answer: 'string', active: false },
		{ id: 2, title: 'string', answer: 'string', active: false }
	];
</script>

<div class="w-full pt-20 pb-6 text-center text-3xl">Classi</div>
<main class="p-4 pt-2">
	{#each faqs as quest, i}
		<div class="active rounded-lg mt-6">
			<button
				on:click={() => (quest.active = !quest.active)}
				class="p-4 lg:p-6 w-full text-start flex justify-between items-center cursor-pointer"
			>
				<span>Lorem ipsum dolor sit amet?</span>
				<span class="transition fas fa-chevron-up {quest.active ? 'rotate-180' : ''}"></span>
			</button>
			{#if quest.active}
				<div
					class="p-4 lg:p-6 shadow dark:shadow-none dark:bg-[#1E2735] rounded-xl"
					transition:slide
				>
					<p class="">
						Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
						incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
						exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat
					</p>
				</div>
			{/if}
		</div>
	{/each}
</main>
