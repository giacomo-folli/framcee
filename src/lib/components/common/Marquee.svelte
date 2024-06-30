<script lang="ts">
	export let reverse: boolean = false,
		pauseOnHover: boolean = false,
		vertical: boolean = false,
		repeat: number = 4;

	let clazz = '';
	export { clazz as class };

	
</script>

<!-- 
  @component
  An infinite scrolling component that can be used to display text, images, or videos.
-->

<div
	class={`group flex overflow-hidden p-2 [--duration:40s] [--gap:1rem] [gap:var(--gap)] ${vertical ? 'flex-col' : 'flex-row'} ${clazz}`}
>
	{#each { length: repeat } as _, i}
		<div
			class={`flex shrink-0 justify-around [gap:var(--gap)] ${vertical ? 'animate-marquee-vertical flex-col' : 'animate-marquee flex-row'} 
            ${pauseOnHover && 'group-hover:[animation-play-state:paused]'} ${reverse && '[animation-direction:reverse]'}`}
		>
			<slot />
		</div>
	{/each}
</div>
