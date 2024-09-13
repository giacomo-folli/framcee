<script lang="ts">
	export let src: string = '',
		alt: string = 'image',
		reversed: boolean = false;

	let clazz = {
		image: ''
	};
	export { clazz as class };
</script>

<section id="text_and_image-{alt}" class="w-full relative px-[25px] py-14 md:pt-24">
	<div
		class="flex flex-col-reverse md:flex-row {reversed
			? ' md:flex-row-reverse '
			: ''} justify-center items-center gap-6 md:gap-10"
	>
		<div class="flex justify-end items-center w-fit">
			<img
				{src}
				{alt}
				class="h-[500px] w-[600px] object-cover rounded-sm shadow-lg {clazz.image}"
			/>
		</div>

		{#if $$slots.text}
			<div class="flex flex-col gap-4 items-start">
				<slot name="text" />
			</div>
		{/if}
	</div>
</section>
