<script lang="ts">
	import { slide } from 'svelte/transition';

	let faqs: {
		title: string;
		answer: string;
		active: boolean;
	}[] = [
		{ title: 'Come ho iniziato', answer: 'string', active: false },
		{ title: 'Esperienze formative', answer: 'string', active: false },
		{ title: 'Esperienze da allenatore', answer: 'string', active: false }
	];
</script>

<div>
	{#each faqs as quest, i}
		<div class="active py-4 {i == 0 ? 'border-y' : 'border-b '} border-slate-300 border-opacity-70">
			<button
				on:click={() => (quest.active = !quest.active)}
				class="p-4 w-full text-start flex justify-between items-center cursor-pointer"
			>
				<span>{quest.title}?</span>
				<span class="transition fas fa-chevron-up {quest.active ? 'rotate-180' : 'rotate-90'}"
				></span>
			</button>
			{#if quest.active}
				<div
					class="p-6"
					transition:slide
				>
					<p>
						Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
						incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
						exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat
					</p>
				</div>
			{/if}
		</div>
	{/each}
</div>
