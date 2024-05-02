<script lang="ts">
	export let src: string,
		rounded: boolean = false,
		width: string | undefined = undefined,
		height: string | undefined = undefined;
</script>

<div
	class="granify overflow-hidden {rounded ? ' rounded-full ' : ''}"
    style:width
    style:height
	style:background-image={`url(${src}),
        url("data:image/svg+xml,%3Csvg viewBox='0 0 400 400' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noiseFilter'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='1.35' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noiseFilter)'/%3E%3C/svg%3E")`}
>
	<!-- <img class="granify" id="img-{alt}" {src} {alt} {width} {height} /> -->
</div>

<style>
	.granify {
		background-position: center;
		background-size: cover;
		background-blend-mode: multiply;
		filter: hue-rotate(-150deg) sepia(100%) contrast(120%) brightness(110%);
		/* background-image: url(/2.png),
			url("data:image/svg+xml,%3Csvg viewBox='0 0 400 400' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noiseFilter'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='1.35' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noiseFilter)'/%3E%3C/svg%3E"); */
	}
</style>
