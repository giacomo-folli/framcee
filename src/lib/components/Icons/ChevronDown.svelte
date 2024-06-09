<script lang="ts">
	export let stroke: string = 'currentColor',
		className: string = 'size-6',
		strokeWidth: string = '1.5';
</script>

<svg
	xmlns="http://www.w3.org/2000/svg"
	fill="none"
	viewBox="0 0 24 24"
	{stroke}
	stroke-width={strokeWidth}
	class={className}
>
	<path stroke-linecap="round" stroke-linejoin="round" d="m19.5 8.25-7.5 7.5-7.5-7.5" />
</svg>
