<script lang="ts">
	import Image from "$lib/components/common/Image.svelte";
</script>

<main class="p-4 text-slate-300">
	<svg height="200px" width="100%">
		<line x1=0 y1=4 x2=400 y2=4/>
		<line x1=0 y1=34 x2=200 y2=34/>
		<line x1=0 y1=64 x2=300 y2=64/>
		<line x1=0 y1=94 x2=280 y2=94/>
        <line x1=0 y1=124 x2=200 y2=124/>
		<line x1=0 y1=154 x2=300 y2=154/>
		<line x1=0 y1=184 x2=280 y2=184/>
	</svg>

	<Image src="/2.png" height="250px" width="250px" />
	<Image src="/logo.png" height="250px" width="250px" />
</main>

<style>
	svg line {
		stroke: currentColor;
		stroke-width: 15;
	}
</style>